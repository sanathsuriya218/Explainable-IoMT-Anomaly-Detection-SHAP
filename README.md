# Explainable Anomaly Detection for IoMT Devices using SHAP

## Overview
This repository contains the implementation of an explainable intrusion detection system for IoMT (Internet of Medical Things) environments using lightweight machine learning models and SHAP-based explainability techniques.

The project focuses on detecting cyber attacks in healthcare IoMT infrastructure while also providing interpretable explanations for model predictions.

The system is evaluated on the CICIoMT2024 benchmark dataset containing network traffic from 40 IoMT devices and 18 attack types.

---

## Features
- Binary anomaly detection for IoMT traffic
- Random Forest and XGBoost classifiers
- SHAP explainability integration
- Per-attack feature importance analysis
- Cross-model SHAP feature agreement
- SHAP stability analysis
- Feature engineering and preprocessing pipeline
- SMOTE-based imbalance handling

---

## Dataset
Dataset Used:
- CICIoMT2024 Dataset

Attack Categories:
- DDoS
- DoS
- MQTT attacks
- Reconnaissance
- Spoofing
- Benign traffic

Dataset Characteristics:
- 8.77M+ records
- 45 network traffic features
- 18 attack types
- 40 IoMT devices

---

## Model Performance

| Model | Accuracy | F1 Score | AUC |
|-------|----------|----------|------|
| Random Forest | 99.90% | 0.9995 | 0.9999 |
| XGBoost | 99.87% | 0.9993 | 1.0000 |

---

## Key Explainability Findings

### DDoS / DoS
- `Rate` is the dominant feature

### Reconnaissance
- `Header Length` strongly influences predictions

### MQTT Attacks
- `IAT` (Inter Arrival Time) is highly significant

### Spoofing
- `Header Length` contributes heavily to attack detection

---

## Project Structure

```bash
├── data/
├── notebooks/
├── models/
├── figures/
├── results/
├── src/
│   ├── preprocessing.py
│   ├── feature_selection.py
│   ├── train_rf.py
│   ├── train_xgb.py
│   ├── shap_analysis.py
│   └── evaluation.py
├── requirements.txt
├── README.md
└── paper.pdf
