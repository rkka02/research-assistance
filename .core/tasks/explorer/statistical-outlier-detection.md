# Statistical Outlier Detection Task - Physics Research

## ⚠️ CRITICAL EXECUTION NOTICE ⚠️

**THIS IS AN EXECUTABLE TASK - NOT REFERENCE MATERIAL**

Apply systematic statistical outlier detection methodology to identify anomalous data points that may indicate measurement errors, systematic effects, or genuine new physics phenomena.

**CORE PRINCIPLE**: Statistical outliers signal important information - systematic detection separates artifacts from discoveries.

## Method Description

**Physics Statistical Outlier Detection System (PSODS)**: Comprehensive outlier detection framework combining univariate and multivariate statistical methods, robust statistics, and physics-informed validation.

**Key Innovation**: Orchestrates multiple statistical approaches while distinguishing measurement artifacts from genuine physics anomalies.

## Statistical Outlier Detection Process

### Phase 1: Data Assessment & Method Selection
1. **Web Search Methodology**: Research optimal outlier detection methods for specific data types
2. **Data Distribution Analysis**: Assess normality, skewness, and distribution characteristics
3. **Outlier Type Assessment**: Identify whether outliers are univariate, multivariate, or contextual
4. **Method Selection**: Choose appropriate detection methods based on data characteristics
5. **Validation Strategy**: Plan independent validation of detected outliers

### Phase 2: Univariate Outlier Detection

#### Standard Statistical Methods
1. **Z-Score Method**:
   ```python
   def z_score_outlier_detection(data, threshold=3.0):
       mean = np.mean(data)
       std = np.std(data)
       z_scores = np.abs((data - mean) / std)
       outliers = data[z_scores > threshold]
       return {
           'outliers': outliers,
           'z_scores': z_scores,
           'threshold': threshold,
           'outlier_indices': np.where(z_scores > threshold)[0]
       }
   ```

2. **Modified Z-Score (Robust)**:
   ```python
   def modified_z_score_detection(data, threshold=3.5):
       median = np.median(data)
       mad = np.median(np.abs(data - median))
       modified_z_scores = 0.6745 * (data - median) / mad
       outliers = data[np.abs(modified_z_scores) > threshold]
       return {
           'outliers': outliers,
           'modified_z_scores': modified_z_scores,
           'mad': mad,
           'outlier_indices': np.where(np.abs(modified_z_scores) > threshold)[0]
       }
   ```

3. **Interquartile Range (IQR) Method**:
   - **Calculation**: Q1 - 1.5×IQR, Q3 + 1.5×IQR boundaries
   - **Mild Outliers**: Outside 1.5×IQR boundaries
   - **Extreme Outliers**: Outside 3×IQR boundaries
   - **Applications**: Non-normal distributions, exploratory analysis

4. **Grubbs' Test**:
   - **Single Outlier Test**: Test most extreme value for outlier status
   - **Test Statistic**: G = max|xi - x̄| / s
   - **Critical Values**: Compare with Grubbs' critical values table
   - **Applications**: Normal distributions, single suspected outlier

### Phase 3: Multivariate Outlier Detection

#### Distance-Based Methods
1. **Mahalanobis Distance**:
   ```python
   def mahalanobis_outlier_detection(data, threshold_percentile=95):
       mean = np.mean(data, axis=0)
       cov = np.cov(data.T)
       inv_cov = np.linalg.inv(cov)
       
       distances = []
       for point in data:
           diff = point - mean
           distance = np.sqrt(diff.T @ inv_cov @ diff)
           distances.append(distance)
       
       threshold = np.percentile(distances, threshold_percentile)
       outliers = data[distances > threshold]
       return {
           'outliers': outliers,
           'distances': distances,
           'threshold': threshold
       }
   ```

2. **Robust Covariance Methods**:
   - **Minimum Covariance Determinant (MCD)**: Robust covariance estimation
   - **Elliptic Envelope**: Robust outlier detection assuming Gaussian distribution
   - **Applications**: Data with multiple outliers affecting covariance structure

#### Machine Learning Methods
1. **Isolation Forest**:
   ```python
   def isolation_forest_detection(data, contamination=0.05):
       from sklearn.ensemble import IsolationForest
       
       detector = IsolationForest(contamination=contamination, random_state=42)
       outlier_labels = detector.fit_predict(data)
       outlier_scores = detector.decision_function(data)
       
       outliers = data[outlier_labels == -1]
       return {
           'outliers': outliers,
           'outlier_scores': outlier_scores,
           'outlier_labels': outlier_labels
       }
   ```

2. **Local Outlier Factor (LOF)**:
   - **Local Density Comparison**: Compare point density with neighbor densities
   - **LOF Score**: LOF > 1.5 typically indicates outliers
   - **Applications**: Data with varying density regions

3. **One-Class SVM**:
   - **Decision Boundary**: Learn boundary around normal data
   - **Kernel Selection**: RBF, polynomial, or linear kernels
   - **Applications**: High-dimensional data, non-linear decision boundaries

### Phase 4: Physics-Informed Outlier Analysis

#### Physics Context Evaluation
1. **Measurement Context Analysis**:
   - **Instrumental Effects**: Could outlier result from detector malfunction?
   - **Environmental Factors**: Unusual environmental conditions during measurement?
   - **Calibration Issues**: Systematic calibration errors affecting specific measurements?
   - **Human Factors**: Observer bias or procedural errors?

2. **Theoretical Context Assessment**:
   - **Known Physics Violations**: Does outlier violate established physics laws?
   - **Theoretical Predictions**: Do theories predict such outlying behavior?
   - **New Physics Potential**: Could outlier indicate beyond-Standard Model physics?
   - **Systematic Effects**: Known systematic effects that could create outliers?

#### Outlier Classification Framework
```python
def classify_physics_outlier(outlier, measurement_context, theoretical_context):
    classification = {
        'type': determine_outlier_type(outlier),
        'physics_significance': assess_physics_significance(outlier, theoretical_context),
        'systematic_probability': estimate_systematic_probability(outlier, measurement_context),
        'discovery_potential': evaluate_discovery_potential(outlier),
        'investigation_priority': calculate_investigation_priority(outlier)
    }
    return classification
```

## Outlier Investigation Protocol

### Immediate Response
1. **Outlier Verification**: Confirm outlier is not due to analysis error
2. **Data Quality Check**: Verify data integrity around outlier occurrence
3. **Method Validation**: Ensure detection method appropriate for data type
4. **Quick Literature Check**: Search for similar outliers in literature

### Systematic Investigation
1. **Reproducibility Testing**: Attempt to reproduce outlying measurements
2. **Systematic Error Analysis**: Comprehensive evaluation of potential systematic causes
3. **Independent Analysis**: Multiple analysis groups examining same data
4. **Expert Consultation**: Domain expert evaluation of outlier significance

### Publication Decision Framework
1. **Statistical Significance**: Meet appropriate significance thresholds
2. **Physics Plausibility**: Assess compatibility with established physics
3. **Systematic Error Probability**: Evaluate likelihood of experimental artifact
4. **Independent Confirmation**: Potential for independent verification

## Quality Control & Validation

### Detection Method Validation
**Method Performance Assessment**:
- **False Positive Rate**: Fraction of normal points incorrectly flagged
- **True Positive Rate**: Fraction of actual outliers correctly identified
- **Precision**: Fraction of flagged points that are genuine outliers
- **Recall**: Fraction of actual outliers successfully detected

**Cross-Method Comparison**:
- **Method Consensus**: Agreement between different detection methods
- **Method Sensitivity**: Ability to detect different types of outliers
- **Method Robustness**: Performance under various data conditions
- **Method Appropriateness**: Suitability for specific physics data types

### Physics Validation Standards
**Conservation Law Compliance**: Verify outliers don't violate fundamental conservation
**Dimensional Consistency**: Check outliers for dimensional consistency
**Theoretical Plausibility**: Assess compatibility with established theory
**Experimental Feasibility**: Evaluate measurement feasibility for outlying values

## Output Format

### Statistical Outlier Detection Report
```yaml
statistical_outlier_detection:
  detection_id: "SOD_{timestamp}"
  dataset_description: "{analyzed dataset characteristics}"
  detection_date: "{analysis completion date}"
  
detection_methods:
  methods_applied: ["{statistical methods used for detection}"]
  method_selection_rationale: "{why specific methods were chosen}"
  parameter_settings: ["{method parameters and threshold values}"]
  
outlier_results:
  total_outliers_detected: "{number of outliers found}"
  outlier_percentage: "{percentage of total data points}"
  detection_consensus: "{agreement between different methods}"
  
outlier_analysis:
  - outlier_id: "OUT001"
    data_value: "{outlying data point or vector}"
    detection_methods: ["{methods that identified this outlier}"]
    statistical_significance: "{deviation magnitude and p-value}"
    physics_context: "{physics interpretation and significance}"
    investigation_priority: "{high|medium|low}"
    
validation_assessment:
  method_performance: "{assessment of detection method effectiveness}"
  cross_validation_results: "{stability of outlier detection across data subsets}"
  physics_consistency: "{compliance with physics principles}"
  literature_comparison: "{comparison with reported outliers in literature}"
  
investigation_recommendations:
  immediate_analysis: ["{outliers requiring immediate investigation}"]
  systematic_investigation: ["{outliers requiring comprehensive analysis}"]
  expert_consultation: ["{outliers requiring domain expert input}"]
  follow_up_experiments: ["{experiments to validate or explain outliers}"]
  
quality_assessment:
  false_positive_risk: "{estimated probability of false outlier detection}"
  detection_completeness: "{estimated fraction of true outliers detected}"
  method_appropriateness: "{suitability of methods for data characteristics}"
  validation_confidence: "{confidence in outlier detection results}"
```

## Integration with Korean Philosophy

### 이상 현상의 체계적 탐구 (Systematic Investigation of Anomalous Phenomena)
- Transform statistical outliers into systematic research opportunities
- Apply methodical analysis to understand outlier significance
- Balance statistical rigor with openness to genuine anomalies

### 건설적 의심 (Constructive Doubt)
- Question outlier significance while investigating potential
- Apply healthy skepticism to outlier interpretations
- Use systematic analysis to distinguish artifacts from discoveries

This statistical outlier detection framework enables systematic identification and analysis of anomalous data points while maintaining scientific rigor and physics interpretability.