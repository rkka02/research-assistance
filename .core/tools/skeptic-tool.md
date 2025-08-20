# skeptic-tool.md
# 레이의 검증 도구함 - Physics Validation & Critical Analysis Tools

## Logical Fallacy Detection System

### Physics-Specific Fallacy Detection
**Dimensional Inconsistency Detection**:
- Automatic dimensional analysis validation: [M L T I Θ N J] consistency check
- Unit conversion verification across measurement systems
- Scale mixing detection: inappropriate micro→macro principle application
- Equation balance verification: dimensional homogeneity in all terms

**Authority and Circular Reasoning Detection**:
- Appeal to authority without evidence analysis
- Circular logic in theoretical frameworks  
- False dichotomy in model comparisons
- Correlation vs causation confusion in physics relationships

### Systematic Logic Verification
**Consistency Checking Framework**:
```
Level 1: Internal Logic - 이론 내부의 논리적 일관성
Level 2: Mathematical Consistency - 수학적 모델의 모순 검사
Level 3: Physical Consistency - 물리 법칙 위반 여부
Level 4: Empirical Consistency - 관찰 데이터와의 일치성
```

**Extreme Case Analysis**:
- Limiting behavior verification: v→c, ℏ→0, G→0 등
- Boundary condition testing: 알려진 결과로의 환원 확인
- Fermi estimation validation: 결과의 order-of-magnitude 합리성
- Conservation law compliance: 에너지, 운동량, 각운동량 보존

## Statistical Rigor Verification Tools

### P-Hacking Detection Framework  
**P-Curve Analysis**:
- Right-skewed curve detection for genuine effects
- Suspicious clustering around p=0.05 identification
- Multiple hypothesis testing without correction flagging
- Selective stopping and optional stopping detection

**Publication Bias Assessment**:
- Funnel plot asymmetry analysis using Egger's test
- File-drawer problem detection via fail-safe N calculation
- Trim-and-fill method for missing studies estimation
- Meta-analysis bias correction techniques

### Multi-Testing Correction Validation
**Look-Elsewhere Effect Control**:
- Global vs local significance distinction in particle physics
- Bonferroni correction verification for multiple comparisons
- False Discovery Rate (FDR) control using Benjamini-Hochberg
- Trial factor correction for data snooping

**Effect Size vs Statistical Significance**:
- Cohen's d calculation and interpretation guidelines
- Confidence interval analysis beyond p-values
- Practical significance assessment in physics contexts
- Bayes factor computation for hypothesis comparison

## Systematic Error Analysis Tools

### Experimental Bias Detection
**Instrumental Bias Identification**:
- Zero-point drift detection in measurement systems
- Scale factor error analysis across instruments
- Hysteresis effect identification in equipment response
- Cross-calibration inconsistency detection

**Observer and Confirmation Bias Detection**:
- Blind analysis protocol verification
- Cherry-picking pattern identification in data selection
- Post-hoc hypothesis formation detection
- Analysis shopping and specification curve analysis

### Data Quality Assessment
**Anomaly vs Artifact Discrimination**:
```python
def anomaly_classification():
    if systematic_pattern_detected():
        return "potential_artifact"
    elif random_fluctuation():
        return "statistical_noise"  
    elif physics_violation():
        return "measurement_error"
    else:
        return "genuine_anomaly"
```

**Reproducibility Verification**:
- Independent replication requirement assessment
- Statistical power analysis for replication studies
- Meta-analytic combination of replication attempts
- Robustness testing across different experimental conditions

## Critical Thinking Framework for Physics

### Dimensional Analysis Verification (Rayleigh Method)
**Systematic Dimensional Checking**:
- Complete variable identification: all relevant physical quantities
- Dimension matrix construction: [M^a L^b T^c I^d Θ^e N^f J^g]
- Rank analysis for dimensional independence
- Pi-theorem application for dimensionless parameter identification

**Physical Scaling Validation**:
- Scaling law verification: power-law relationship confirmation
- Similarity analysis: model-prototype scaling consistency
- Regime identification: different physics at different scales
- Scale separation verification: clear hierarchy confirmation

### Symmetry and Conservation Law Verification
**Noether's Theorem Applications**:
- Continuous symmetry→conservation law mapping verification
- Symmetry breaking analysis and consequence assessment
- Gauge invariance checking in field theories
- Discrete symmetry verification: parity, time-reversal, charge conjugation

**Conservation Law Compliance Testing**:
```yaml
conservation_checks:
  energy: "∂H/∂t = 0 for time-independent Hamiltonians"
  momentum: "∂L/∂x = 0 → p_x = constant"
  angular_momentum: "spherical symmetry → L conservation"
  charge: "gauge symmetry → Q conservation"
```

## Alternative Hypothesis Generation

### Competing Model Assessment Framework
**Model Selection Criteria**:
- Akaike Information Criterion (AIC) comparison
- Bayesian Information Criterion (BIC) evaluation  
- Cross-validation performance assessment
- Occam's razor application: simplicity vs explanatory power balance

**Falsifiability Testing**:
- Testable prediction identification for each model
- Crucial experiment design for model discrimination
- Risk assessment: what observations would falsify the theory?
- Popper's demarcation criterion application

### Counterfactual Analysis Engine
**What-If Scenario Generation**:
- Assumption relaxation: "What if conservation law X didn't hold?"
- Parameter space exploration: extreme limit behavior analysis
- Causal inference testing: intervention vs correlation distinction
- Alternative mechanism identification: different explanatory pathways

## Automated Validation Systems

### NLP-Based Assumption Detection
**Hidden Assumption Identification**:
- Implicit premise extraction from physics papers using fine-tuned language models
- Assumption dependency tree construction
- Circular reasoning detection in theoretical frameworks
- Tacit knowledge identification requiring explicit justification

**Literature Cross-Validation**:
- Citation network analysis for authority cluster detection
- Replication crisis pattern identification across fields
- Retraction database integration for red flag identification
- Consensus vs evidence distinction in scientific literature

### Machine Learning Bias Detection
**Training Data Bias Identification**:
- Sample selection bias in physics datasets
- Measurement bias propagation through ML pipelines
- Algorithmic fairness assessment in physics applications
- Out-of-distribution generalization testing

**Model Interpretability Requirements**:
- Physics-informed explainable AI implementation
- Feature importance validation against physical intuition
- Adversarial example generation for robustness testing
- Uncertainty quantification in ML-assisted physics

## Reproducibility Assessment Framework

### Computational Reproducibility
**Code Review and Verification**:
- Numerical algorithm stability analysis
- Random seed dependency testing
- Compiler and hardware independence verification
- Version control and dependency management assessment

**Data Provenance Tracking**:
- Complete experimental parameter logging
- Data preprocessing step documentation
- Statistical analysis pipeline verification
- Result sensitivity analysis to parameter variations

### Experimental Reproducibility Standards
**Protocol Verification Framework**:
```yaml
reproducibility_checklist:
  materials: "Complete equipment and material specifications"
  methods: "Step-by-step procedural documentation"  
  conditions: "Environmental parameter recording"
  calibration: "Instrument calibration protocols"
  controls: "Positive and negative control inclusion"
  statistics: "Sample size justification and power analysis"
```

## Real-Time Validation Monitoring

### Continuous Quality Assurance
**Anomaly Detection in Research Workflow**:
- Statistical outlier detection in experimental data streams
- Pattern recognition for systematic errors
- Early warning systems for confirmation bias
- Real-time p-hacking detection during analysis

### Collaborative Skepticism Tools
**Distributed Peer Review Systems**:
- Adversarial collaboration framework implementation
- Anonymous critical review integration
- Prediction market for research outcome validation
- Crowd-sourced replication effort coordination

### Emergency Validation Protocols
**Crisis Response Framework**:
- Rapid independent verification procedures
- Emergency replication study coordination
- Community-wide validation mobilization
- Media and public communication protocols during controversies

## Integration with Team Validation

### Cross-Agent Verification
**Explorer-Skeptic Dialectic**:
- Discovery claim verification pipeline
- Novelty vs artifact discrimination protocol
- Serendipity validation framework
- Innovation protection while maintaining rigor

**Architect-Skeptic Structural Review**:
- Framework robustness testing
- Systematic weakness identification
- Alternative architecture evaluation
- Structural assumption validation

### Quality Gate Implementation
**Multi-Level Validation Checkpoints**:
- Preliminary analysis quality gates
- Intermediate result verification points
- Final publication readiness assessment
- Post-publication monitoring systems