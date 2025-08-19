# Uncertainty Calculator Utility - Physics Research

## ⚠️ CRITICAL UTILITY TOOL ⚠️

**THIS IS A UTILITY TOOL - Used by Craftsman agent for systematic uncertainty calculation**

Advanced uncertainty calculation algorithms implementing JCGM 100:2008 standards for comprehensive uncertainty analysis in physics research.

```python
class PhysicsUncertaintyCalculator:
    def __init__(self):
        self.standards = {
            'confidence_levels': [0.68, 0.95, 0.99],
            'coverage_factors': {'95%': 2.0, '99%': 3.0},
            'correlation_threshold': 0.1
        }
        
    def calculate_comprehensive_uncertainty(self, measurement_data, systematic_sources):
        # Type A (statistical) uncertainty
        type_a = self.calculate_type_a_uncertainty(measurement_data)
        
        # Type B (systematic) uncertainty
        type_b = self.calculate_type_b_uncertainty(systematic_sources)
        
        # Combined uncertainty
        combined = self.combine_uncertainties(type_a, type_b)
        
        # Expanded uncertainty
        expanded = self.calculate_expanded_uncertainty(combined)
        
        return {
            'type_a': type_a,
            'type_b': type_b, 
            'combined': combined,
            'expanded': expanded,
            'uncertainty_budget': self.create_uncertainty_budget(type_a, type_b)
        }
        
    def propagate_uncertainty(self, function, variables, uncertainties, correlations=None):
        # Linear propagation for simple cases
        if self.is_linear_function(function):
            return self.linear_uncertainty_propagation(function, variables, uncertainties, correlations)
        
        # Monte Carlo propagation for complex cases
        else:
            return self.monte_carlo_uncertainty_propagation(function, variables, uncertainties, correlations)
            
    def monte_carlo_uncertainty_propagation(self, function, variables, uncertainties, correlations, n_samples=100000):
        # Generate correlated random samples
        samples = self.generate_correlated_samples(variables, uncertainties, correlations, n_samples)
        
        # Evaluate function for all samples
        function_values = [function(*sample) for sample in samples]
        
        # Calculate uncertainty from sample distribution
        return {
            'mean': np.mean(function_values),
            'standard_uncertainty': np.std(function_values),
            'confidence_intervals': {
                '68%': np.percentile(function_values, [16, 84]),
                '95%': np.percentile(function_values, [2.5, 97.5]),
                '99%': np.percentile(function_values, [0.5, 99.5])
            },
            'distribution_shape': self.analyze_distribution_shape(function_values)
        }
```

This uncertainty calculator provides comprehensive JCGM 100:2008 compliant uncertainty analysis for physics research applications.