# HCV Assay Evaluation — Simulated Diagnostic Performance Analysis

A Python-based simulation and diagnostic performance evaluation of a Hepatitis C Core Antigen assay versus Nucleic Acid Amplification Testing (NAAT), modeled after published clinical research including a multi-center study in *Microbiology Spectrum* (2024).

---

## Overview

This project simulates a real-world HCV diagnostic assay evaluation study using probabilistic data generation and standard clinical performance metrics. It covers the full data science lifecycle: data simulation, exploratory analysis, feature engineering, and algorithm evaluation.

Discordant cases (false negatives at low viral loads) are deliberately engineered to reflect a known clinical limitation of antigen-based assays — particularly relevant to treatment monitoring populations.

---

## Key Results

| Metric | Value |
|---|---|
| Sensitivity | 96.6% |
| Specificity | 100.0% |
| Overall Concordance | 97.3% |
| Cohen's Kappa | 0.914 |
| Discordant Cases | 14 / 512 specimens |
| Discordance Pattern | All false negatives at viral loads 500–5,000 IU/mL |

---

## Dataset Structure

Two linked relational datasets:

- **Patient-level** (n = 450): patient ID, age, sex
- **Specimen-level** (n = 512): specimen ID, patient ID, specimen type (Screening/Monitoring), collection date, viral load, NAAT result, antigen signal, antigen result

---

## Methods

- Probabilistic data simulation (numpy: normal, log-normal, rule-based discordant case injection)
- Exploratory data analysis
- Diagnostic performance evaluation: sensitivity, specificity, concordance, confusion matrix
- Agreement analysis: Cohen's kappa (scikit-learn)
- Visualization: viral load distribution, viral load vs. antigen signal (log-scaled), confusion matrix heatmap

---

## Tech Stack

Python · pandas · numpy · scikit-learn · matplotlib · Jupyter Notebook

---

## Clinical Context

Inspired by contributed research on HCV antigen assay performance in a U.S. population:

> Degaga B. et al. *Comparison of a Hepatitis C Core Antigen Assay to Nucleic Acid Amplification Testing for Detection of HCV Viremia in a U.S. Population.* Microbiology Spectrum, 2024. Poster presented at AACC Annual Scientific Meeting & Clinical Lab Expo, 2023.

---

## Author

**Biniam Degaga** — M.S. Data Science candidate | Medical Laboratory Scientist  
[LinkedIn](https://www.linkedin.com/in/) <!-- add your LinkedIn URL -->
