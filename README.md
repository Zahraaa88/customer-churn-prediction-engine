# 🛒 E-Commerce & Subscription Customer Churn Prediction Engine
**Author:** Zahra Moradi (Commercial & Data Analyst)  
**Tech Stack:** Python (Pandas, Scikit-Learn, Seaborn, Matplotlib) • Gradient Boosting / XGBoost • Exploratory Data Analysis (EDA) • Statistical Modeling

---

## 📌 Executive Summary & Business Dilemma
In high-velocity subscription and e-commerce platforms, customer attrition silently bleeds annual recurring revenue. Most growth and operations teams react to churn **after** the subscription is cancelled.

This project delivers an **end-to-end predictive machine learning engine** analyzing **16,093 customer accounts** to identify friction points and predict churn with a **99.63% Test Accuracy (99.99% ROC-AUC)**, allowing customer success teams to intervene proactively.

---

## 📊 Key Analytical Insights & Root Cause Drivers
* **Payment Friction is the #1 Churn Signal:** Customers with **>18 days billing delay** exhibited a **+0.57 correlation with churn**, making payment friction responsible for **45.8% of model feature importance**.
* **Support Contact Surge:** Accounts reaching **≥5 support calls** had a dramatic spike in cancellation probability (**15.5% feature importance**).
* **Contract Vulnerability:** Monthly subscription agreements experienced higher churn rates (**51.2%**) compared to quarterly and annual commitments (**44.0% - 46.7%**).

---

## 🤖 Model Benchmarking (5-Fold Cross-Validation)

| Algorithm | CV ROC-AUC (Train) | Test Accuracy | Test ROC-AUC | Test F1-Score | Status |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Logistic Regression (Baseline)** | 90.95% | 82.01% | 89.87% | 81.40% | Linear Baseline |
| **Random Forest Classifier** | 99.99% | 99.38% | 99.99% | 99.34% | High Performer |
| **Gradient Boosting Classifier** | **99.99%** | **99.63%** | **99.99%** | **99.61%** | 🏆 **Best Model** |

---

## 🧩 Confusion Matrix Performance (3,219 Test Samples)
```
                  Predicted Retained (0)   Predicted Churned (1)
Actual Retained (0)       1,692                    3
Actual Churned (1)           9                   1,515
```
* **True Positives:** 1,515 at-risk customers successfully flagged before leaving.
* **Precision:** 0.99 (Near-zero false alarms).
* **Recall:** 0.99 (99% of churning accounts captured).

---

## 📁 Repository Structure
```
├── data/
│   └── blinkit_churn_2025.csv          # 16,093 customer records
├── notebooks/
│   └── 01_churn_prediction_engine.ipynb # Complete EDA, modeling & inference
└── README.md                            # Executive case study documentation
```

---

## 📬 Contact & Opportunities
Open to international remote Commercial Data Analyst roles and consulting engagements.
* **LinkedIn:** [linkedin.com/in/zahra-moradi88](https://www.linkedin.com/in/zahra-moradi88/)
