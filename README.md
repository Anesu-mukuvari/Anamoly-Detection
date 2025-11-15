# Time-Series Anomaly Detection: Rolling-Window and Z-Score Methods

This project applies advanced time-series analysis for anomaly detection in business and financial datasets. The goal: improve a baseline anomaly model by engineering a rolling-window, Z-score based detection process and validate its robustness on both real and synthetic data.

## Project Overview

- **Objective:** Enhance a baseline anomaly detector (85% accuracy) for time-series data by introducing local rolling statistics and statistical normalization.
- **Challenge:** Only one cell in the model could be edited, requiring efficient, creative use of the code interface (engineering under constraints).
- **Context:** Applications include fraud/outlier detection in finance, operations, IoT, sensor monitoring, and system health.

## Methodology

- **Baseline model:** Used Isolation Forest and simple differencing, sensitive to global scale.
- **Improved model:**
  - Employs a rolling window (7 observations) to compute local mean and std.
  - Calculates Z-scores for differenced values, standardizing anomaly magnitude.
  - Selects as anomaly the max Z-score index (statistically significant outlier).
  - Tuned window size for optimal generalization.
- **Validation:** Model performance tested on both original and synthetically generated series mimicking trend, noise, and anomalous behaviors.

## Results

- **Baseline accuracy:** 85%
- **Improved model:** 93% accuracy on both original and synthetic datasets.
- Demonstrates generalization, robust detection, and reduced sensitivity to non-anomalous scale jumps.

## Skills Demonstrated

- Python time-series analysis (pandas, NumPy, scikit-learn)
- Statistical anomaly detection/engineering
- Rolling statistics, model tuning, synthetic data generation
- Business and finance analytics applications

## Authors

Mukuvari A., Matlhare T.

## License

Academic and educational use only.

---

*This project demonstrates practical time-series anomaly detection and feature engineering for real-world data science and analytics roles.*

