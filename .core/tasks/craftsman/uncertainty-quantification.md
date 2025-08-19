# Uncertainty Quantification Task - Physics Research

## ⚠️ CRITICAL EXECUTION NOTICE ⚠️

**THIS IS AN EXECUTABLE TASK - NOT REFERENCE MATERIAL**

Apply systematic uncertainty quantification methodology following JCGM 100:2008 standards for comprehensive error analysis in physics research.

**CORE PRINCIPLE**: Comprehensive uncertainty quantification enables reliable conclusions - systematic error assessment supports scientific credibility.

## Method Description

**Physics Uncertainty Quantification System (PUQS)**: Complete uncertainty analysis framework combining Type A (statistical) and Type B (systematic) uncertainty evaluation, correlation analysis, and Monte Carlo propagation.

## Uncertainty Quantification Framework

### Phase 1: Uncertainty Source Identification
1. **Web Search Standards**: Research uncertainty quantification best practices for specific physics domain
2. **Error Source Mapping**: Systematic identification of all uncertainty sources
3. **Uncertainty Type Classification**: Categorize as Type A (statistical) or Type B (systematic)
4. **Correlation Assessment**: Identify correlations between uncertainty sources
5. **Traceability Establishment**: Link measurements to fundamental standards

### Phase 2: Type A Uncertainty Evaluation (Statistical)
```python
def calculate_type_a_uncertainty(measurements):
    n = len(measurements)
    mean = np.mean(measurements)
    std_dev = np.std(measurements, ddof=1)  # Sample standard deviation
    
    # Standard uncertainty of the mean
    standard_uncertainty = std_dev / np.sqrt(n)
    
    # Degrees of freedom
    degrees_of_freedom = n - 1
    
    # Coverage factor for desired confidence level
    confidence_level = 0.95
    t_value = stats.t.ppf((1 + confidence_level) / 2, degrees_of_freedom)
    
    return {
        'standard_uncertainty': standard_uncertainty,
        'expanded_uncertainty': standard_uncertainty * t_value,
        'coverage_factor': t_value,
        'degrees_of_freedom': degrees_of_freedom,
        'confidence_level': confidence_level
    }
```

### Phase 3: Type B Uncertainty Evaluation (Systematic)
```python
def calculate_type_b_uncertainty(systematic_sources):
    type_b_components = []
    
    for source in systematic_sources:
        if source['distribution'] == 'rectangular':
            # Uniform distribution: u = a/sqrt(3)
            uncertainty = source['half_width'] / np.sqrt(3)
        elif source['distribution'] == 'triangular':
            # Triangular distribution: u = a/sqrt(6)
            uncertainty = source['half_width'] / np.sqrt(6)
        elif source['distribution'] == 'normal':
            # Normal distribution: u = sigma
            uncertainty = source['standard_deviation']
        
        type_b_components.append({
            'source': source['name'],
            'uncertainty': uncertainty,
            'distribution': source['distribution'],
            'degrees_of_freedom': source.get('degrees_of_freedom', np.inf)
        })
    
    return type_b_components
```

### Phase 4: Combined Uncertainty Calculation
```python
def calculate_combined_uncertainty(type_a_uncertainty, type_b_uncertainties, correlations=None):
    # Combine Type A and Type B uncertainties
    variance_sum = type_a_uncertainty['standard_uncertainty']**2
    
    # Add Type B components
    for type_b in type_b_uncertainties:
        variance_sum += type_b['uncertainty']**2
    
    # Add correlation terms if present
    if correlations is not None:
        correlation_contribution = calculate_correlation_contribution(type_b_uncertainties, correlations)
        variance_sum += correlation_contribution
    
    combined_standard_uncertainty = np.sqrt(variance_sum)
    
    # Calculate effective degrees of freedom (Welch-Satterthwaite equation)
    effective_dof = calculate_effective_degrees_of_freedom(type_a_uncertainty, type_b_uncertainties)
    
    # Coverage factor for expanded uncertainty
    coverage_factor = stats.t.ppf(0.975, effective_dof)  # 95% confidence
    expanded_uncertainty = combined_standard_uncertainty * coverage_factor
    
    return {
        'combined_standard_uncertainty': combined_standard_uncertainty,
        'expanded_uncertainty': expanded_uncertainty,
        'coverage_factor': coverage_factor,
        'effective_degrees_of_freedom': effective_dof,
        'confidence_level': 0.95
    }
```

This uncertainty quantification framework provides systematic JCGM 100:2008 compliant uncertainty analysis for physics research measurements and calculations.