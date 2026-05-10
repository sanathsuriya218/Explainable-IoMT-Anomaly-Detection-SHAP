# NeuroShield-IoMT: Explainable and Uncertainty-Aware Cyber Defense Framework for Medical IoT Networks

## Overview
NeuroShield-IoMT is a next-generation explainable cybersecurity framework designed for securing Internet of Medical Things (IoMT) ecosystems against sophisticated cyber threats.

Unlike traditional intrusion detection systems that operate as black-box classifiers, NeuroShield-IoMT combines:

- Explainable AI (XAI)
- Uncertainty-aware threat scoring
- Multi-stage anomaly reasoning
- Adaptive attack fingerprinting
- Lightweight edge-compatible machine learning

The framework is specifically engineered for healthcare environments where transparency, reliability, and low-latency inference are critical.

The system leverages the CICIoMT2024 benchmark dataset containing network traffic generated from 40 heterogeneous IoMT devices and multiple real-world attack scenarios.

---

# Core Innovations

## 1. Hybrid Explainable Threat Intelligence Engine
The framework integrates:
- Random Forest Ensembles
- XGBoost Gradient Boosting
- SHAP Explainability
- Dynamic Feature Attribution

This enables both:
- high-performance attack detection
- interpretable forensic analysis

---

## 2. Uncertainty-Aware Risk Scoring
Instead of generating binary predictions alone, the system computes:

- Confidence Scores
- Prediction Entropy
- Feature Contribution Variance
- Attack Certainty Levels

This allows:
- reliable threat prioritization
- false positive reduction
- clinical-grade trustworthiness

---

## 3. Multi-Level Attack Fingerprinting
NeuroShield-IoMT introduces hierarchical attack fingerprinting:
- Protocol-level signatures
- Temporal traffic signatures
- Statistical flow signatures
- Explainability-driven feature patterns

Each attack category develops a unique behavioral fingerprint.

---

## 4. Cross-Model Explainability Consensus
The framework performs explainability agreement analysis between:
- Random Forest
- XGBoost

This identifies:
- stable cybersecurity indicators
- robust attack discriminators
- model-independent threat signatures

---

## 5. SHAP Stability Validation
A novel explanation stability engine validates whether feature attributions remain stable across:
- random subsamples
- varying traffic distributions
- noisy attack environments

This improves reliability for real-world deployment in healthcare systems.

---

# Dataset

## CICIoMT2024 Benchmark Dataset

### Dataset Characteristics
- 8.77M+ network flow records
- 45 traffic features
- 40 IoMT devices
- 18 cyberattack types
- Multi-protocol traffic generation

### Attack Categories
- DDoS Flooding
- TCP/UDP DoS
- MQTT Flooding
- Reconnaissance
- ARP Spoofing
- Port Scanning
- Vulnerability Scanning
- ICMP Attacks
- Benign Healthcare Traffic

---

# System Architecture

```text
IoMT Traffic
      ↓
Flow Extraction Engine
      ↓
Feature Engineering Pipeline
      ↓
Adaptive Preprocessing Layer
      ↓
Hybrid ML Detection Core
      ↓
SHAP Explainability Engine
      ↓
Uncertainty Quantification Layer
      ↓
Threat Intelligence Dashboard
