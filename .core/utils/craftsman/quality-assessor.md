# Quality Assessor Utility - Physics Research

## ⚠️ CRITICAL UTILITY TOOL ⚠️

**Used by Craftsman agent for systematic quality assessment**

```python
class PhysicsQualityAssessor:
    def __init__(self, domain_standards):
        self.standards = domain_standards
        
    def assess_implementation_quality(self, implementation_data, context):
        quality_scores = {
            'precision_achievement': self.measure_precision_quality(implementation_data),
            'accuracy_validation': self.validate_accuracy_quality(implementation_data),
            'reproducibility_score': self.assess_reproducibility_quality(implementation_data),
            'documentation_quality': self.evaluate_documentation_completeness(implementation_data),
            'standards_compliance': self.check_standards_compliance(implementation_data, context)
        }
        
        overall_quality = self.calculate_weighted_quality_score(quality_scores)
        
        return {
            'overall_quality': overall_quality,
            'component_scores': quality_scores,
            'quality_grade': self.assign_quality_grade(overall_quality),
            'improvement_recommendations': self.generate_improvement_suggestions(quality_scores)
        }
        
    def continuous_quality_monitoring(self, measurement_stream):
        quality_history = []
        
        for measurement in measurement_stream:
            instant_quality = self.assess_measurement_quality(measurement)
            quality_history.append(instant_quality)
            
            if self.quality_alert_needed(instant_quality):
                yield self.generate_quality_alert(instant_quality, measurement)
                
        return self.summarize_quality_performance(quality_history)
```

This quality assessor provides comprehensive quality evaluation capabilities for physics research implementations.