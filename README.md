# ALLOCENTRIC BUT NOT EGOCENTIC NAVIGATION IS DISRUPTED BY ACUTE HYPOXIA

## Overview

This repository contains the data and analysis code used to investigate how acute continuous hypoxia (ACH) and acute intermittent hypoxia (AIH) influence:

1. Spatial navigation performance (SPACE)
2. Resting-state EEG activity
3. Relationships between physiological responses to hypoxia and behavioural/neurophysiological outcomes

---

## Repository Structure

```text
OXYNAV/
│
├── data/
│   ├── MASTER_CHANGE_WITH_SPO2.csv
│   ├── SpO2_continuous.csv
│   └── SpO2_intermittent.csv
│
├── notebooks/
│   ├── eeg_processing.ipynb
│   ├── hypothesis1_navigation.ipynb
│   ├── hypothesis2_eeg.ipynb
│   └── hypothesis3_spo2.ipynb
│
├── results/
│
├── requirements.txt
│
└── README.md
```

## Data Files

### MASTER_CHANGE_WITH_SPO2.csv

Primary analysis dataset containing:

- Navigation outcomes
- EEG metrics
- SpO₂ measures
- Intervention information
- Session information

### SpO2_continuous.csv

Physiological recordings collected during Acute Continuous Hypoxia (ACH).

### SpO2_intermittent.csv

Physiological recordings collected during Acute Intermittent Hypoxia (AIH).

## Hypotheses

### Hypothesis 1

Acute hypoxia impairs navigational performance.

Outcomes:

- Path Integration
- Egocentric Pointing
- Mapping
- Perspective-Taking

Models:

- Linear Mixed Models (REML)
- Generalised Estimating Equations (GEE)

### Hypothesis 2

Acute hypoxia alters intrinsic brain activity.

Measures:

- Alpha power
- Alpha central frequency
- Beta power
- Beta central frequency
- Aperiodic exponent
- Aperiodic offset

### Hypothesis 3

The magnitude of oxygen desaturation predicts behavioural and EEG outcomes.

Predictors:

- SpO₂
- Intervention

## EEG Processing

EEG preprocessing was performed using:

- MNE-Python
- PREP Pipeline
- ICA
- ICLabel
- AutoReject

Spectral parameterisation was performed using Specparam (formerly FOOOF).

## Reproducibility

All analyses were conducted in Python.

Model diagnostics included:

- Residual histograms
- Q-Q plots
- Residual vs fitted plots
- Shapiro-Wilk tests

Outliers were removed using a ±3 SD criterion before model fitting.

## Data Availability

This repository contains processed datasets required to reproduce the analyses reported in the associated manuscript.

Raw EEG recordings are not included in this repository.
