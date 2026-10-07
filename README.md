# Customer Churn Prediction

## 📌 Project Overview
This project implements a Machine Learning pipeline to predict customer churn using historical usage, contract, and billing data. By identifying potential churners in advance, organizations can deploy proactive retention strategies to improve customer lifetime value and minimize revenue drop-off.

## 🛠️ Preprocessing & Methodology
- **Data Cleaning:** Processed numerical variables, handled missing values, and parsed `TotalCharges`.
- **Feature Encoding:** Encoded categorical features and binary targets using `LabelEncoder`.
- **Feature Scaling:** Standardized feature distributions using `StandardScaler`.
- **Stratified Split:** Executed an 80/20 train-test split maintaining class balance.

## 📊 Model Evaluation & Benchmarking
Evaluated three classification algorithms based on Accuracy and Recall:

| Model | Accuracy | Recall (Churn) | Precision | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | **79.39%** | **56.42%** | **62%** | **0.59** |
| Random Forest | 78.18% | 47.86% | 62% | 0.54 |
| XGBoost | 77.33% | 52.67% | 58% | 0.55 |

> **Key Finding:** **Logistic Regression** achieved the highest overall accuracy (79.39%) and recall (56.42%), making it the most effective model for identifying at-risk customers.

## 🔑 Key Risk Factors
Feature importance analysis identified primary drivers behind churn:
- **Tenure Length:** Shorter customer relationship history strongly correlates with higher churn probability.
- **Contract Type:** Month-to-month contracts pose significantly higher risk compared to annual plans.
- **Monthly Charges:** High recurring charges serve as a key trigger for customer drop-off.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/Ramana171807/Customer-Churn-Prediction.git](https://github.com/Ramana171807/Customer-Churn-Prediction.git)
