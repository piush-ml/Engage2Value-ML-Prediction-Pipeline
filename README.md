# Engage2Value – Purchase Value Prediction (ML Project)

## Overview

Engage2Value is a machine learning project focused on predicting customer **purchaseValue** based on multi-session behavioral data from a digital commerce platform. The project uses session metrics, device attributes, traffic sources, and geographical indicators to model user purchase potential.

The workflow follows a complete end-to-end ML pipeline including data loading, EDA, preprocessing, model building, hyperparameter tuning, and model comparison, evaluated using the **R² score** as per the competition objective.

---

## Project Structure

```
Engage2Value/
│
├── Data/
│   ├── train.csv
│   ├── test.csv
│   └── sample_submission.csv
│
├── notebook/
│   └── multi-session-purchase-value-prediction.ipynb
│
└── Engage2Value-Project-Report.pdf
```

* **Data/** – Contains training, test, and submission datasets
* **notebook/** – Jupyter notebook with full ML pipeline
* **Project Report** – Detailed academic report based on notebook analysis

---

## Problem Statement

The goal is to predict a customer’s **purchaseValue** using anonymized multi-session interaction data including:

* User engagement metrics (totalHits, pageViews, visits)
* Device and browser information
* Traffic and marketing sources
* Geographical attributes

This is a supervised regression problem evaluated using **R² score** between predicted and actual values.

---

## Dataset Description

Each row represents a unique user session from a digital commerce platform and includes:

* Behavioral features (session activity & engagement)
* Device and technical attributes
* Traffic acquisition channels
* Geographic context
* Target variable: `purchaseValue`

The dataset is high-dimensional with:

* 37 categorical features
* Skewed numerical distributions
* High missing values in some traffic-related columns

---

## Methodology

The notebook follows a structured ML workflow:

1. Data Loading & Understanding
2. Exploratory Data Analysis (EDA)
3. Categorical & Numerical Feature Analysis
4. Outlier Study
5. Data Preprocessing (Encoding, Scaling, Pipeline)
6. Model Building (Regression Models)
7. Hyperparameter Tuning
8. Model Comparison (based on R² score)

A preprocessing pipeline is used to handle missing values, encode categorical variables, and prevent data leakage.

---

## Key Insights

* The target variable `purchaseValue` is highly skewed with many zero-value sessions
* Engagement metrics like **pageViews** and **totalHits** strongly influence purchase behavior
* Several advertising-related columns contain >90% missing values
* Chrome dominates browser usage, indicating platform concentration
* High-cardinality categorical features significantly impact model complexity

---

## Models Used

* Tree-based Regression Models (Ensemble Methods)
* Pipeline-based preprocessing + modeling approach
* Hyperparameter tuning for improved generalization

These models were selected due to their robustness on high-dimensional tabular data and ability to capture non-linear relationships.

---

## Evaluation Metric

Model performance is evaluated using:

> **R² Score**

---

## Applications

* Customer value prediction
* Marketing optimization
* Revenue forecasting
* User segmentation and personalization

---

## Author

**Piush Das**
Machine Learning Project – Engage2Value
Predicting Purchase Value from Multi-Session Behavioral Data
