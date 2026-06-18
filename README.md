# Customer-Retention
ML model predicting customer churn using Python and scikit-learn.

# Customer Churn Prediction & Retention Analysis

 **Predicting customer churn using machine learning to enable proactive retention strategies.**

---

## 📌 Project Overview

Customer churn is one of the most critical business problems — acquiring a new customer costs **5-25x more** than retaining an existing one. This project builds an end-to-end machine learning pipeline to predict which customers are at risk of leaving, identify key churn drivers, and provide actionable business insights for retention teams.

**Business Problem:** A telecom/subscription-based company wants to move from reactive (customer already left) to proactive (predict & prevent) retention.

**Solution:** A classification model that predicts churn probability with interpretable feature importance, enabling targeted retention campaigns.

---

## 🗂️ Dataset

| Feature | Description |
|---------|-------------|
| `customerID` | Unique identifier |
| `gender`, `SeniorCitizen`, `Partner`, `Dependents` | Demographics |
| `tenure` | Months with the company |
| `PhoneService`, `MultipleLines`, `InternetService` | Service subscriptions |
| `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies` | Add-on services |
| `Contract`, `PaperlessBilling`, `PaymentMethod` | Billing & contract details |
| `MonthlyCharges`, `TotalCharges` | Financial metrics |
| `Churn` | **Target:** Yes/No (customer left or not) |

**Source:** [IBM Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) 

---

## 🔬 Methodology

### 1. Exploratory Data Analysis (EDA)
- Univariate & bivariate analysis of churn drivers
- Correlation heatmaps & distribution plots
- Identified class imbalance (~26% churn rate)

### 2. Data Preprocessing
- Handled missing values (`TotalCharges` coercion)
- Encoded categorical variables (One-Hot Encoding)
- Feature scaling (StandardScaler)


### 3. Model Evaluation
- **Confusion Matrix** analysis
- **ROC-AUC Curve** for threshold tuning
- **Precision-Recall Trade-off** (critical for imbalanced data)
- **Cross-validation** for robustness

### 4. Feature Importance & Interpretability
- Top churn predictors identified:
  1. **Contract Type** (Month-to-month = high risk)
  2. **Tenure** (New customers churn more)
  3. **Monthly Charges** (Higher charges → higher churn)
  4. **Tech Support** (Lack of support drives churn)
  5. **Online Security** (No security = more churn)

---

## 🛠️ Tech Stack

[Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-1.5+-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-1.23+-013243?logo=numpy)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.2+-F7931E?logo=scikit-learn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.6+-11557c?logo=matplotlib)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-4c72b0?logo=seaborn)


## Linkedin Profile:
https://www.linkedin.com/in/mannatpreet-kaur-3360303b9/
