# Statistical Inference Toolkit

> Linear regression, hypothesis testing, and confidence intervals — derived from scratch, validated against sklearn.

**Live Project Page:** [coyjohnson25.github.io/statistical-inference-lab](https://coyjohnson25.github.io/statistical-inference-lab)  
**Portfolio:** [coyjohnson25.github.io](https://coyjohnson25.github.io)

---

## Overview

Most data scientists reach for sklearn immediately. This project takes the opposite approach — every statistical method is derived mathematically before a single line of code is written. The goal is to prove these aren't black boxes, but logical consequences of well-understood probability theory.

---

## What's Inside

```
statistical-inference-lab/
├── README.md
├── requirements.txt
├── notebooks/
│   └── statistical_inference.ipynb    ← Full walkthrough
├── src/
│   ├── linear_regression.py           ← OLS from scratch
│   ├── hypothesis_tests.py            ← t-tests, F-tests, chi-square
│   ├── confidence_intervals.py        ← CI construction
│   └── diagnostics.py                 ← Residual analysis
├── results/
│   ├── residual_plots.png
│   └── comparison_table.png
└── docs/
    └── index.html                     ← Project detail page
```

---

## Methods Implemented

| Method | Description |
|--------|-------------|
| OLS Linear Regression | Closed-form solution via normal equations β̂ = (XᵀX)⁻¹Xᵀy |
| Hypothesis Testing | t-tests, F-tests, p-value computation from scratch |
| Confidence Intervals | Two-sided CIs using t-distribution critical values |
| Residual Diagnostics | Breusch-Pagan, Shapiro-Wilk, Durbin-Watson tests |

---

## Key Math

```
# Ordinary Least Squares — closed-form solution
β̂ = (XᵀX)⁻¹ Xᵀy

# t-statistic for H₀: βⱼ = 0
t = β̂ⱼ / SE(β̂ⱼ),   t ~ t(n - p - 1)

# 95% Confidence Interval
CI = β̂ ± t_{α/2, n-p-1} · SE(β̂)
```

---

## Quickstart

```bash
git clone https://github.com/coyjohnson25/statistical-inference-lab.git
cd statistical-inference-lab
pip install -r requirements.txt
jupyter notebook notebooks/statistical_inference.ipynb
```

---

## Results

- 100% match with sklearn coefficients, standard errors, and p-values
- 5 diagnostic tests implemented for assumption checking
- Validated across 3 real-world datasets

---

## Tech Stack

`Python` `R` `NumPy` `SciPy` `Statsmodels` `Jupyter`

---

## Author

**Coy Johnson** — [coyjohnson25@gmail.com](mailto:coyjohnson25@gmail.com)  
M.S. Mathematics Candidate | Applied Mathematician