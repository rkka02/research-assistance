# Similarity Calculator Utility - Physics Research

## ⚠️ CRITICAL UTILITY TOOL ⚠️

**Used by Explorer agent for systematic similarity quantification**

Advanced similarity calculation algorithms for comparing physics phenomena, theories, and data across domains.

```python
class PhysicsSimilarityCalculator:
    def calculate_similarity(self, object1, object2, similarity_type='comprehensive'):
        if similarity_type == 'mathematical':
            return self.mathematical_similarity(object1, object2)
        elif similarity_type == 'phenomenological':
            return self.phenomenological_similarity(object1, object2)
        elif similarity_type == 'structural':
            return self.structural_similarity(object1, object2)
        else:
            return self.comprehensive_similarity(object1, object2)
            
    def mathematical_similarity(self, eq1, eq2):
        return {
            'equation_structure': self.compare_equation_structure(eq1, eq2),
            'symmetry_similarity': self.compare_symmetries(eq1, eq2),
            'solution_similarity': self.compare_solutions(eq1, eq2),
            'dimensional_similarity': self.compare_dimensions(eq1, eq2)
        }
```

This similarity calculator provides quantitative similarity assessment for cross-domain physics research.