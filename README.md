# NCAA Football Predictive Analytics

## Overview

This project develops a predictive analytics framework for NCAA FBS football games using ELO ratings, moving-average performance metrics, and machine learning models.

The objective is to improve game outcome prediction accuracy by combining team performance history, rolling statistical features, and calibrated probability modeling.

The project was developed as part of analytical research work associated with the Kissell Research Group.

---

# Business Problem

Sports organizations, analysts, and betting markets rely heavily on predictive models to evaluate team strength and forecast game outcomes.

Traditional win-loss statistics often fail to capture:

* momentum shifts,
* recent performance trends,
* home-field advantage,
* and long-term team strength.

This project addresses these limitations by integrating:

* ELO rating systems,
* rolling performance averages,
* and machine learning classification models.

---

# Objectives

* Build an NCAA football game prediction model
* Optimize ELO rating parameters
* Evaluate rolling-average feature combinations
* Compare predictive model performance
* Improve probability calibration and prediction reliability

---

# Project Workflow

1. Data collection and preprocessing
2. ELO rating calculation
3. Feature engineering
4. Moving-average window optimization
5. Model training and calibration
6. Performance evaluation

---

# Methodology

## ELO Rating System

The project implemented a customized ELO framework with:

* K-factor tuning
* home-field advantage adjustments
* mean reversion
* rating damping

A grid search process was used to identify the best parameter combination.

### Best ELO Configuration

| Parameter      | Value |
| -------------- | ----- |
| K-Factor       | 25    |
| Home Advantage | 100   |
| Mean Reversion | 0.10  |
| Damping        | 0.70  |

---

# Feature Engineering

Features included:

* rolling average points scored
* rolling average points allowed
* rolling average margin
* rolling win rate
* ELO rating differential
* home/away indicators

Moving-average windows tested:

* 3-game
* 5-game
* 7-game combinations

---

# Models Used

* Logistic Regression
* Calibrated Classification Models
* Huber Regressor

---

# Evaluation Metrics

* Accuracy
* Calibration Performance
* Out-of-Sample Prediction
* Probability Reliability

---

# Key Insights

* ELO parameter tuning significantly improved predictive stability
* Combining rolling performance metrics with ELO features improved model accuracy
* Probability calibration improved prediction reliability for close-match games
* Recent team momentum contributed strongly to predictive performance

---

# Tools & Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Jupyter Notebook

---

# Repository Structure

```text
data/           Raw and processed datasets
notebooks/      Jupyter notebooks
src/             Python scripts for modeling
outputs/         Generated predictions and reports
images/          Visualizations and charts
docs/             Supporting documentation
```

---

# Future Improvements

* Integrate betting market odds
* Add player-level statistics
* Explore XGBoost and ensemble methods
* Deploy an interactive dashboard for real-time predictions

---

# Author

Po An Tao
M.S. Business Analytics — George Washington University
