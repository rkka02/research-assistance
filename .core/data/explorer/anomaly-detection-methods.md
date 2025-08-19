# Anomaly Detection Methods - Physics Research Library

## ⚠️ CRITICAL DATA REFERENCE ⚠️

**THIS IS A REFERENCE DATA FILE - Used by Explorer agent for systematic anomaly detection**

Comprehensive library of anomaly detection methods optimized for physics research contexts, including statistical approaches, machine learning techniques, and physics-informed detection algorithms.

**CORE PRINCIPLE**: Systematic anomaly detection separates breakthrough discoveries from experimental artifacts.

## Statistical Anomaly Detection Methods

### Univariate Statistical Methods
**Z-Score Analysis**:
- **Method**: Identify data points >3 standard deviations from mean
- **Formula**: z = (x - μ) / σ
- **Threshold**: |z| > 3 for outlier classification
- **Applications**: Gaussian-distributed physics measurements, experimental outlier detection
- **Limitations**: Assumes normal distribution, sensitive to extreme outliers

**Modified Z-Score (Robust)**:
- **Method**: Use median absolute deviation instead of standard deviation
- **Formula**: M = 0.6745(x - median) / MAD
- **Threshold**: |M| > 3.5 for outlier classification
- **Applications**: Non-Gaussian physics data, robust outlier detection
- **Advantages**: Resistant to extreme outliers, works with skewed distributions

**Interquartile Range (IQR) Method**:
- **Method**: Flag points outside Q1 - 1.5×IQR to Q3 + 1.5×IQR
- **Calculation**: IQR = Q3 - Q1, bounds = [Q1-1.5×IQR, Q3+1.5×IQR]
- **Applications**: Physics data with unknown distributions, exploratory analysis
- **Advantages**: Distribution-free, intuitive interpretation

**Grubbs' Test**:
- **Method**: Statistical test for single outliers in normal distributions
- **Test Statistic**: G = max|xi - x̄| / s
- **Applications**: Physics experiments with single suspected outliers
- **Limitations**: Assumes normal distribution, tests only most extreme outlier

### Multivariate Statistical Methods
**Mahalanobis Distance**:
- **Method**: Account for correlations between variables in outlier detection
- **Formula**: DM = √[(x - μ)ᵀ Σ⁻¹ (x - μ)]
- **Threshold**: Chi-square distribution with degrees of freedom = number of variables
- **Applications**: Correlated physics variables, multi-parameter experiments
- **Advantages**: Accounts for variable correlations and different scales

**Robust Covariance Estimation**:
- **Method**: Use minimum covariance determinant for outlier-resistant analysis
- **Applications**: Physics data with multiple outliers affecting covariance structure
- **Algorithms**: Minimum Covariance Determinant (MCD), Robust Principal Components
- **Advantages**: Resistant to outlier contamination in covariance estimation

## Machine Learning Anomaly Detection

### Unsupervised Learning Approaches
**Isolation Forest**:
- **Principle**: Isolate anomalies using random forest approach
- **Algorithm**: Recursive random partitioning, shorter paths indicate anomalies
- **Parameters**: n_estimators=100, contamination=0.01-0.05
- **Applications**: High-dimensional physics data, mixed data types
- **Advantages**: Efficient, works with mixed data types, minimal parameter tuning

**One-Class Support Vector Machine (OCSVM)**:
- **Principle**: Learn decision boundary around normal data in high-dimensional space
- **Kernel Options**: RBF, polynomial, linear kernels for different data characteristics
- **Parameters**: nu parameter controls outlier fraction (typically 0.01-0.05)
- **Applications**: Complex physics parameter spaces, non-linear relationships
- **Advantages**: Effective in high dimensions, flexible kernel choices

**DBSCAN Clustering**:
- **Principle**: Density-based clustering identifying noise points as anomalies
- **Parameters**: eps (neighborhood radius), min_samples (minimum cluster size)
- **Anomaly Criterion**: Points not belonging to any cluster (labeled as noise)
- **Applications**: Spatial physics data, event clustering in particle physics
- **Advantages**: Finds arbitrarily shaped clusters, automatic outlier identification

**Local Outlier Factor (LOF)**:
- **Principle**: Compare local density of point with local densities of neighbors
- **Calculation**: LOF = average(local_density_neighbors) / local_density_point
- **Threshold**: LOF > 1.5 typically indicates outliers
- **Applications**: Physics data with varying density regions
- **Advantages**: Adapts to local data density, finds outliers in dense regions

### Deep Learning Approaches
**Autoencoders for Anomaly Detection**:
- **Architecture**: Encoder: Input → 512 → 256 → 128 → 64, Decoder: 64 → 128 → 256 → 512 → Output
- **Training**: Train on normal data only, high reconstruction error indicates anomalies
- **Threshold**: Typically 95th or 99th percentile of reconstruction errors
- **Applications**: High-dimensional physics data, complex non-linear relationships
- **Advantages**: Captures complex patterns, works with mixed data types

**Variational Autoencoders (VAE)**:
- **Principle**: Probabilistic reconstruction with uncertainty quantification
- **Anomaly Score**: Combination of reconstruction error and KL divergence
- **Applications**: Physics data requiring uncertainty quantification
- **Advantages**: Provides uncertainty estimates, generates synthetic normal data

**Deep Support Vector Data Description (Deep SVDD)**:
- **Principle**: Learn minimal hypersphere containing normal data
- **Training**: Minimize hypersphere volume while containing training data
- **Applications**: Complex physics patterns requiring non-linear boundaries
- **Advantages**: Combines deep learning with principled anomaly detection

## Physics-Informed Anomaly Detection

### Conservation Law Violation Detection
**Energy Conservation Monitoring**:
- **Method**: Track energy balance in physics simulations and experiments
- **Violation Threshold**: |ΔE| > 3σ_measurement for potential anomalies
- **Applications**: Particle collisions, nuclear reactions, quantum systems
- **Systematic Checks**: Verify energy accounting includes all relevant forms

**Momentum Conservation Analysis**:
- **Method**: Vector sum of momenta before and after interactions
- **Violation Criterion**: |Δp| > √(Σσ²) for anomaly flagging
- **Applications**: Collision experiments, scattering processes
- **Cross-Validation**: Multiple detector subsystems for verification

**Charge Conservation Verification**:
- **Method**: Track total charge through all physics processes
- **Applications**: Particle physics, plasma physics, electrochemistry
- **Anomaly Indicators**: Apparent charge creation or destruction

### Symmetry Violation Detection
**Gauge Invariance Testing**:
- **Method**: Verify physics results independent of gauge choice
- **Implementation**: Test multiple gauge configurations for consistency
- **Applications**: Electromagnetic theory, Yang-Mills theories
- **Anomaly Indicators**: Gauge-dependent physics predictions

**Lorentz Invariance Verification**:
- **Method**: Test special relativity compliance in high-energy experiments
- **Applications**: Particle physics, precision tests of relativity
- **Violation Signatures**: Frame-dependent physics results

**Discrete Symmetry Analysis**:
- **Parity (P)**: Space inversion symmetry testing
- **Time Reversal (T)**: Time reversal symmetry verification
- **Charge Conjugation (C)**: Particle-antiparticle symmetry analysis
- **Combined Tests**: CPT theorem verification

### Scale-Specific Anomaly Detection
**Quantum Scale Anomalies**:
- **Coherence Loss**: Unexpected decoherence in quantum systems
- **Entanglement Anomalies**: Non-classical correlations exceeding theoretical limits
- **Tunneling Anomalies**: Barrier penetration differing from quantum predictions
- **Measurement Anomalies**: Quantum measurement results violating theoretical expectations

**Classical Scale Anomalies**:
- **Trajectory Deviations**: Classical motion differing from Newtonian predictions
- **Field Anomalies**: Classical field behavior violating Maxwell equations
- **Thermodynamic Anomalies**: Heat flow violating thermodynamic laws
- **Mechanical Anomalies**: Force-acceleration relationships deviating from F=ma

**Cosmological Scale Anomalies**:
- **Dark Matter Signatures**: Gravitational effects without visible matter
- **Dark Energy Indicators**: Accelerating expansion beyond matter/radiation content
- **Large-Scale Structure**: Cosmic web patterns differing from predictions
- **Cosmic Microwave Background**: Temperature fluctuation anomalies

## Specialized Detection Algorithms

### Time Series Anomaly Detection
**Change Point Detection**:
- **CUSUM Algorithm**: Cumulative sum for detecting mean shifts
- **Bayesian Change Point**: Probabilistic change point identification
- **Applications**: Long-term physics measurements, equipment monitoring

**Seasonal Decomposition**:
- **STL Decomposition**: Separate trend, seasonal, and residual components
- **Anomaly Detection**: Flag unusual residual patterns
- **Applications**: Cyclical physics phenomena, environmental measurements

**ARIMA-Based Detection**:
- **Model Fitting**: Fit ARIMA model to normal time series
- **Prediction Intervals**: Flag points outside prediction confidence bands
- **Applications**: Stationary physics time series with autocorrelation

### Spatial Anomaly Detection
**Spatial Clustering**:
- **DBSCAN**: Density-based clustering for spatial outlier detection
- **K-Nearest Neighbors**: Local density comparison for spatial anomalies
- **Applications**: Detector hit patterns, astronomical object distributions

**Image-Based Anomaly Detection**:
- **Convolutional Autoencoders**: Learn normal image patterns, flag deviations
- **Template Matching**: Compare experimental images with theoretical expectations
- **Applications**: Detector images, astronomical observations, microscopy

### Network-Based Anomaly Detection
**Graph Anomaly Detection**:
- **Community Detection**: Identify unusual community structures
- **Centrality Anomalies**: Nodes with unexpected centrality measures
- **Applications**: Citation networks, collaboration networks, interaction networks

**Dynamic Network Anomalies**:
- **Temporal Network Analysis**: Detect unusual evolution patterns
- **Link Prediction**: Identify unexpected or missing connections
- **Applications**: Evolving research networks, dynamic interaction systems

## Validation and Quality Control

### Method Validation Framework
**Cross-Validation**:
- **K-Fold Validation**: Test method performance on held-out data
- **Time Series Split**: Temporal validation for time-dependent data
- **Spatial Validation**: Geographic or detector-based validation splits

**Performance Metrics**:
- **True Positive Rate**: Fraction of actual anomalies correctly identified
- **False Positive Rate**: Fraction of normal points incorrectly flagged
- **Precision**: Fraction of flagged points that are genuine anomalies
- **Recall**: Fraction of actual anomalies successfully detected
- **F1-Score**: Harmonic mean of precision and recall

### Physics-Specific Validation
**Domain Expert Review**: Subject matter expert evaluation of detected anomalies
**Literature Cross-Check**: Comparison with previously reported anomalies
**Systematic Error Assessment**: Evaluation of potential experimental artifacts
**Reproducibility Testing**: Independent confirmation of anomaly detection

## Integration Guidelines

### Explorer Agent Usage
- **Systematic Scanning**: Apply multiple methods for comprehensive anomaly detection
- **Method Selection**: Choose appropriate methods based on data characteristics
- **Validation Pipeline**: Systematically validate detected anomalies
- **Discovery Integration**: Transform validated anomalies into research discoveries

### Quality Assurance Integration
- **Method Comparison**: Compare results across different detection methods
- **Threshold Optimization**: Adjust detection thresholds based on domain requirements
- **Performance Monitoring**: Track detection accuracy and false positive rates
- **Continuous Improvement**: Refine methods based on validation outcomes

This anomaly detection methods library provides systematic approaches for identifying unexpected phenomena while distinguishing genuine discoveries from experimental artifacts and noise.