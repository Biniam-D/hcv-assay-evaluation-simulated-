# HCV Assay Evaluation — Simulated Diagnostic Performance Analysis

This project simulates an HCV diagnostic assay evaluation using Python. It compares a Hepatitis C Core Antigen assay to Nucleic Acid Amplification Testing (NAAT) as the reference method, based on real published research.

---

## What This Project Does

- Generates a simulated patient and specimen dataset
- Assigns viral loads, antigen signals, and test results
- Introduces false negatives at low viral loads to reflect a known real-world limitation
- Evaluates how well the antigen assay agrees with NAAT using standard diagnostic metrics

---

## Key Results

| Metric | Value |
|---|---|
| Sensitivity | 96.6% |
| Specificity | 100.0% |
| Overall Concordance | 97.3% |
| Cohen's Kappa | 0.914 |
| Discordant Cases | 14 out of 512 specimens |

All discordant cases were false negatives occurring at low viral loads (500–5,000 IU/mL).

---

## Data

Two simulated datasets:

- **Patients** (n = 450): ID, age, sex
- **Specimens** (n = 512): specimen type, collection date, viral load, NAAT result, antigen signal, antigen result

---

## Tools Used

Python · pandas · numpy · scikit-learn · matplotlib · Jupyter Notebook

---

## Background

This simulation is based on a study I contributed to:

> Degaga B. et al. *Comparison of a Hepatitis C Core Antigen Assay to Nucleic Acid Amplification Testing for Detection of HCV Viremia in a U.S. Population.* Microbiology Spectrum, 2024. Poster presented at AACC Annual Scientific Meeting, 2023.

---
Author
**Biniam Degaga** — M.S. Data Science candidate | Medical Laboratory Scientist  

