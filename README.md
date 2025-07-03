# 🧠 LASSO & Ridge Regression Examples

This repository provides Python implementations of **LASSO** (Least Absolute Shrinkage and Selection Operator) and **Ridge** regression, along with practical demonstrations, dataset usage, model evaluation, and visualization.

---

## 📋 Table of Contents

1. [Overview](#overview)
2. [Algorithms](#algorithms)
3. [Dataset](#dataset)
4. [Getting Started](#getting-started)
   - [Requirements](#requirements)
   - [Installation](#installation)
5. [Usage](#usage)
   - [LASSO Regression](#lasso-regression)
   - [Ridge Regression](#ridge-regression)
   - [Comparing Models](#comparing-models)
6. [Results & Plots](#results--plots)
7. [Performance Metrics](#performance-metrics)
8. [Contributing](#contributing)
9. [References](#references)
10. [License](#license)

---

## 🌟 Overview

This project demonstrates:
- **LASSO Regression**: uses L1 penalty to encourage sparsity—useful for feature selection.
- **Ridge Regression**: uses L2 penalty to shrink coefficients and mitigate multicollinearity.

Ideal for those learning about:
- Regularized linear models.
- Practical implementation with `scikit-learn`.
- Visualizing bias–variance trade-offs.

---

## 🔬 Algorithms

- **LASSO**: minimizes the sum of squared errors with an L1 norm penalty:  
  $$\min_{\beta} \left\{ \|y - X\beta\|_2^2 + \alpha \|\beta\|_1 \right\}$$  
- **Ridge**: minimizes the sum of squared errors with an L2 norm penalty:  
  $$\min_{\beta} \left\{ \|y - X\beta\|_2^2 + \alpha \|\beta\|_2^2 \right\}$$  

Tuning the penalty parameter `α` controls complexity and helps prevent overfitting.

---

## 📊 Dataset

This repo uses a synthetic dataset (via `sklearn.datasets.make_regression`) with configurable:
- `n_samples`
- `n_features`
- `noise`
- `effective_features`

You can easily swap in your own data (CSV, database, etc.)—just adjust the loader code accordingly.

---

## 🚀 Getting Started

### Requirements

- Python 3.7+
- Pip

### Installation

```sh
git clone https://github.com/KodaliSuchitraKamala/LASSO_And_Ridge_Regressions.git
cd LASSO_And_Ridge_Regressions
pip install -r requirements.txt
