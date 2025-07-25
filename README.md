# 🏈 NFL Combine Analysis with Linear Regression

## Overview

This project uses **multiple linear regression** to predict a football player's **40-yard dash time** based on metrics collected at the NFL Combine.

---

## Dataset

- **Source**: `NFLcombine.csv` (Kaggle)
- **Target Variable**: `Forty` (40-yard dash time in seconds)
- **Features Used**:
  - `Ht` – Height (inches)
  - `Wt` – Weight (lbs)
  - `Vertical` – Vertical jump (inches)
  - `BroadJump` – Broad jump (inches)
  - `Cone` – 3-cone drill time (seconds)
  - `Shuttle` – 20-yard shuttle time (seconds)

---

## Methods

- Data cleaning and preprocessing with `pandas`
- Exploratory analysis with `seaborn.pairplot()`
- Linear model fitting using `scikit-learn` library

---

## Performance Metrics

| Metric                     | Value   |
|----------------------------|---------|
| **R² Score (Test)**        | 0.864   |
| **Mean Squared Error (MSE)** | 0.0134  |
| **Cross-Validation (5-fold)** | 0.858   |

---

## Assumptions of Linearity

- **Pairplot**: Understand pairwise relationships between features and the target
- **Residual Plot**: Check for homoscedasticity (constant variance of errors)
- **Q-Q Plot**: Validate the normality of residuals

---

