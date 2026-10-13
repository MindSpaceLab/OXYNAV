# Acute Hypoxia Disrupts Multiple Processes Supporting Spatial Navigation

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
│   ├── behavioural_eeg_data.csv
│   ├── SpO2_continuous.csv
│   └── SpO2_intermittent.csv
│
├── notebooks/
│   ├── ART ANOVA.Rmd
│   
│
│
└── README.md
```

## Data Files

### behavioural_eeg_data.csv

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

All analyses were conducted in R and available in ART ANOVA.Rmd

## Data Availability

This repository contains processed datasets required to reproduce the analyses reported in the associated manuscript.

Raw EEG recordings are not included in this repository.
