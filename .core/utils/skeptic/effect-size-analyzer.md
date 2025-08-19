# Effect Size Analyzer Utility

## Overview
**Purpose**: Systematic calculation and interpretation of effect sizes in physics research to assess practical significance beyond statistical significance

**Effect Size Philosophy**: "효과 크기가 진정한 중요성을 말해준다" (Effect size tells us true importance)

---

## Effect Size Analysis Framework

### 1. Effect Size Selection and Calculation
**Method**: Choosing and computing appropriate effect size measures for physics research

#### Effect Size Categories:
```yaml
effect_size_calculation:
  standardized_effect_sizes:
    cohen_d_family:
      - cohen_d_calculation: "Mean difference divided by pooled standard deviation"
      - hedges_g_correction: "Bias-corrected version for small samples"
      - glass_delta_application: "When variances are markedly different"
      - appropriate_usage_conditions: "Normal distributions, homogeneous variances"
    
    correlation_based_measures:
      - pearson_r_effect_size: "Linear relationship strength"
      - spearman_rho_application: "Non-parametric relationship assessment"
      - point_biserial_correlation: "Dichotomous-continuous relationships"
      - eta_squared_variance_explained: "Proportion of variance explained"
  
  physics_specific_measures:
    measurement_based_effects:
      - signal_to_noise_ratio: "Detection capability assessment"
      - measurement_precision_improvement: "Relative precision enhancement"
      - systematic_error_reduction: "Bias reduction quantification"
      - uncertainty_reduction_factor: "Precision improvement measure"
    
    theoretical_significance:
      - dimensionless_parameter_changes: "Fundamental constant modifications"
      - symmetry_breaking_magnitude: "Deviation from exact symmetry"
      - approximation_accuracy_improvement: "Model refinement benefits"
      - predictive_power_enhancement: "Forecasting capability improvement"
```

### 2. Effect Size Interpretation Framework
**System**: Contextual interpretation of effect sizes in physics research

#### Interpretation Guidelines:
```yaml
effect_size_interpretation:
  magnitude_benchmarks:
    cohen_conventions:
      - small_effect: "d = 0.2, r = 0.1, η² = 0.01"
      - medium_effect: "d = 0.5, r = 0.3, η² = 0.06"
      - large_effect: "d = 0.8, r = 0.5, η² = 0.14"
      - context_dependent_interpretation: "Physics-specific benchmarks preferred"
    
    physics_domain_benchmarks:
      - measurement_precision: "Relative to current measurement capabilities"
      - theoretical_predictions: "Relative to theoretical uncertainty"
      - experimental_sensitivity: "Relative to detection thresholds"
      - practical_applications: "Relative to technological requirements"
  
  confidence_intervals:
    effect_size_uncertainty:
      - confidence_interval_calculation: "Bootstrap or analytical methods"
      - uncertainty_propagation: "From measurement to effect size"
      - robustness_assessment: "Sensitivity to outliers and assumptions"
      - replication_probability: "Expected effect size in replication"
    
    practical_significance:
      - minimum_detectable_effect: "Smallest meaningful effect size"
      - cost_benefit_thresholds: "Economic significance boundaries"
      - technological_impact_levels: "Application-relevant effect sizes"
      - scientific_advancement_criteria: "Knowledge progress thresholds"
```

### 3. Meta-Analysis Integration
**Application**: Effect size synthesis across multiple studies

#### Meta-Analysis Framework:
```yaml
meta_analysis_integration:
  effect_size_synthesis:
    fixed_effects_model:
      - weighted_average_calculation: "Precision-weighted effect size"
      - homogeneity_testing: "Q-statistic and I² assessment"
      - publication_bias_detection: "Funnel plot analysis"
      - sensitivity_analysis: "Influence of individual studies"
    
    random_effects_model:
      - between_study_variance: "Heterogeneity quantification"
      - prediction_intervals: "Future study effect size prediction"
      - moderator_analysis: "Subgroup effect differences"
      - mixed_effects_modeling: "Continuous moderator integration"
  
  quality_assessment_integration:
    study_quality_weighting:
      - methodological_quality_scores: "Design quality assessment"
      - risk_of_bias_evaluation: "Systematic bias impact"
      - precision_based_weighting: "Measurement quality consideration"
      - relevance_scoring: "Applicability to research question"
```

---

This effect size analyzer utility enables comprehensive assessment of practical significance in physics research, maintaining the principle that "효과 크기가 진정한 중요성을 말해준다" (effect size tells us true importance).