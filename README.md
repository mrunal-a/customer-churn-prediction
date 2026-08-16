# Customer Churn Prediction & Analytics

## 📌 Project Overview

Customer churn prediction is a machine learning project that identifies customers who are likely to stop using a company's services.

This project combines:

- Exploratory Data Analysis
- SQL-based customer analysis
- Machine Learning
- Customer risk segmentation
- Power BI dashboard
- Streamlit prediction application

The goal is to help businesses identify high-risk customers and take proactive retention actions.

---

## 🎯 Objectives

- Analyze customer churn patterns
- Identify factors associated with churn
- Build machine learning models to predict churn
- Compare Logistic Regression, Random Forest and XGBoost
- Identify high-risk and high-value customers
- Build an interactive business dashboard
- Build a real-time churn prediction application

---

## 📊 Dataset

The project uses the Telco Customer Churn dataset.

Important features include:

- Gender
- SeniorCitizen
- Partner
- Dependents
- Tenure
- PhoneService
- InternetService
- OnlineSecurity
- OnlineBackup
- DeviceProtection
- TechSupport
- StreamingTV
- StreamingMovies
- Contract
- PaperlessBilling
- PaymentMethod
- MonthlyCharges
- TotalCharges

Target variable:

`Churn`

---

## 🛠️ Technologies Used

### Programming
- Python

### Data Analysis
- Pandas
- NumPy
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn
- XGBoost

### Database / Analysis
- SQL

### Visualization
- Power BI

### Deployment
- Streamlit

### Model Storage
- Joblib

---

## 🤖 Machine Learning Models

Three classification models were evaluated:

1. Logistic Regression
2. Random Forest
3. XGBoost

### XGBoost Performance

| Metric | Score |
|---|---:|
| Accuracy | 80.41% |
| Precision | 66.23% |
| Recall | 53.48% |
| F1-Score | 59.17% |
| ROC-AUC | 84.50% |

XGBoost achieved the highest ROC-AUC among the evaluated models.

Random Forest achieved higher recall, making it useful when identifying as many potential churners as possible is the primary business objective.

---

## 📈 Business Insights

The analysis identified several important churn patterns:

- Month-to-month customers have substantially higher churn.
- Customers with shorter tenure are more likely to churn.
- Electronic check users show relatively high churn.
- High monthly charges can be associated with increased churn risk.
- High-risk and high-value customers can be prioritized for retention campaigns.

---

## ⭐ High-Risk Customer Prioritization

The project combines:

- Churn probability
- Customer value

to identify customers who are both:

**High Risk + High Value**

These customers can be prioritized for targeted retention strategies.

---

## 📊 Power BI Dashboard

The dashboard contains:

- Total Customers
- Churned Customers
- Churn Rate
- High-Risk Customers
- High-Risk + High-Value Customers
- Churn by Contract
- Churn by Payment Method
- Churn by Tenure
- High-Risk Customer Table

---

## 🚀 Streamlit Application

The Streamlit application allows users to enter customer information and receive:

- Churn Probability
- Risk Level
- Prediction Result

Risk levels are categorized as:

- LOW
- MEDIUM
- HIGH

---

## 📁 Project Structure

```text
customer-churn-prediction/
│
├── app/
│   └── app.py
│
├── data/
│   ├── raw/
│   └── processed/
│
├── models/
│   └── xgboost_churn_model.pkl
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_machine_learning.ipynb
│   ├── 03_sql_analysis.ipynb
│   └── 04_machine_learning.ipynb
│
├── README.md
└── requirements.txt