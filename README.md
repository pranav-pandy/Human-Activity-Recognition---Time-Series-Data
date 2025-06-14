# ⏱️ Human Activity Recognition Using Time Series Classification

This project focuses on the classification of human physical activities using time-series data collected from wearable sensors. The goal is to accurately identify different activities based on statistical time-domain features extracted from multivariate sensor readings.

---

## 📚 Overview

Human activity data is collected from a wireless sensor network and includes six time-series signals per instance. The project involves:

- Extracting meaningful time-domain features from raw time series
- Building binary and multiclass classification models
- Evaluating model performance using ROC, AUC, and cross-validation

---

## 📁 Dataset

- **Source**: [UCI AReM Dataset](https://archive.ics.uci.edu/ml/datasets/Activity+Recognition+system+based+on+Multisensor+data+fusion+%28AReM%29)
- **Activities**: Walking, Sitting, Standing, Lying, Bending1, Bending2, Cycling
- **Structure**:
  - 88 instances across 7 activity folders
  - Each instance contains 6 time series of 480 readings each
  - Signals include: avg_rss12, var_rss12, avg_rss13, var_rss13, avg_rss23, var_rss23

---

## ⚙️ Feature Extraction

Statistical time-domain features were computed for each of the 6 time series in every instance:

- Minimum, Maximum, Mean, Median
- Standard Deviation, First Quartile, Third Quartile

The resulting feature matrix is used for training classification models.

---

## 🤖 Models Used

### Binary Classification
- Logistic Regression
- L2-Regularized Logistic Regression
- Recursive Feature Elimination (RFE) for feature pruning
- Cross-validation for model robustness

### Multiclass Classification
- Multinomial Logistic Regression
- Evaluated with and without standardized features

---

## 📈 Evaluation

- ROC Curve and AUC Score
- Confusion Matrix
- Feature Importance via p-values and RFE
- Performance comparison between 6 vs. 12 segmented time series

---

## 🔍 Key Highlights

- Applied time-domain statistical techniques for effective feature engineering
- Implemented dynamic segmentation for enhanced temporal resolution
- Used recursive feature elimination and p-value selection for dimensionality reduction
- Achieved reliable classification performance with interpretability

---

## 🧩 Tech Stack

- Python (NumPy, Pandas, Matplotlib, Scikit-learn)
- Jupyter Notebook for development and experimentation

---
