# Comparative Evaluation of Logistic Regression and Linear Discriminant Analysis Using Simulation and Real-World Health Data

## Overview

This project investigates the performance of **Logistic Regression** and **Linear Discriminant Analysis (LDA)** for binary classification under different statistical conditions using both Monte Carlo simulation and real-world health data.

The study was motivated by understanding how model assumptions, sample characteristics, predictor relationships, and data-generating mechanisms influence classification performance in statistical learning problems.

---

## Research Objectives

- Compare the predictive performance of Logistic Regression and Linear Discriminant Analysis under controlled simulation settings.
- Evaluate how sample size, predictor correlation, and class separation affect classification accuracy.
- Apply both methods to real-world health data from the **2022 Bangladesh Demographic and Health Survey (BDHS)** for hypertension classification.
- Investigate the impact of statistical assumptions and sampling design on inference and predictive evaluation.

---

## Methodology

### 1. Monte Carlo Simulation Study

A simulation framework was developed to compare Logistic Regression and LDA under varying:

- Sample sizes
- Predictor correlations
- Degree of class separation

Performance was evaluated using:

- Area Under the ROC Curve (AUC/C-index)
- Q-index
- B-index
- ROC analysis
- Resampling-based uncertainty assessment

---

### 2. Real-World Application: BDHS Hypertension Classification

Both classification approaches were applied to the **2022 Bangladesh Demographic and Health Survey (BDHS)** to predict hypertension status using demographic and health-related predictors.

The analysis involved:

- Exploratory data analysis
- Variable construction
- Model fitting and comparison
- Predictive performance evaluation
- Assessment of uncertainty through resampling methods

---

## Statistical Reflection

During further evaluation of the analysis, I identified an important methodological limitation regarding bootstrap inference.

Because BDHS follows a **clustered survey sampling design**, conventional individual-level bootstrap resampling does not preserve the dependence structure introduced by the sampling clusters. A cluster-level bootstrap approach would provide a more appropriate framework by resampling at the level of primary sampling units and maintaining the underlying survey structure.

This experience strengthened my understanding that statistical methods must be evaluated within the context of how data are generated, collected, and structured.

---

## Skills and Tools

**Statistical Methods**
- Logistic Regression
- Linear Discriminant Analysis
- Monte Carlo Simulation
- Bootstrap Methods
- ROC Analysis
- Classification Performance Evaluation

**Programming**
- R

**Data Analysis**
- Exploratory Data Analysis
- Statistical Modeling
- Health Data Analysis
- Survey Data Considerations

---

## Dataset

**Bangladesh Demographic and Health Survey (BDHS) 2022**

The dataset was used to investigate hypertension classification using real-world population health data.

*(Raw survey data are not included due to data-sharing restrictions.)*

---

## Key Learning Outcomes

This project provided experience in:

- Understanding model assumptions beyond algorithmic performance
- Evaluating statistical methods through simulation
- Applying classification methods to complex health datasets
- Recognizing the importance of sampling design and dependence structures in statistical inference
