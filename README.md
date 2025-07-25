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

## Conclusions

- Assumptions of Linearity are upheld
- 86.4% of variability is explained by the model
- The feature variables well-explain 40-yard dash time, indicating a strong linear relationship between the combine metrics and 40-yard dash performance

---

## Future Insight

This linear regression model performs well, explaining ~ 86% of the variance in 40-yard dash times with low error and interpretable results, making it a strong baseline. However, it may miss non-linear relationships and interaction effects. In the future, I should explore regularization and tree-based models for improved accuracy.
