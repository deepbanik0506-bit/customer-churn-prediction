# 📊 Customer Churn Prediction

## 🎯 Project Overview
This project builds a machine learning model to predict customer churn for a telecom company.

Customer churn directly impacts recurring revenue. The goal is to identify customers likely to leave so that targeted retention strategies can be applied.

---

## 🧠 Problem Statement
Customer churn leads to revenue loss. From a business perspective:

- False Negatives (missed churners) → Lost customers → Revenue loss  
- False Positives (incorrect churn prediction) → Unnecessary retention cost  

The model must balance churn detection with operational constraints.

---

## 📁 Dataset
Synthetic Telecom Customer Churn Dataset (100,000 records).

Features include:
- Age
- Tenure
- Monthly Charges
- Total Charges
- Contract Type
- Payment Method
- Gender

Target:
`Churn (Yes / No)`

---

## ⚙️ Methodology

- Data cleaning & preprocessing  
- One-hot encoding for categorical variables  
- Stratified train-test split (80/20)  
- Logistic Regression & Random Forest models  
- Class imbalance handling  
- Decision threshold tuning  
- Model evaluation using precision, recall, F1-score  

---

## 🏆 Final Model

**Balanced Logistic Regression (threshold = 0.5)**

Accuracy: ~69%  
Recall (Churn): ~70%  
Precision (Churn): ~52%  

Lowering the threshold to 0.4 increased recall to ~82%, demonstrating the trade-off between detecting churners and minimizing false positives.

---

## 📌 Key Insight

Customers with short-term contracts are significantly more likely to churn.  
Longer contract durations and higher tenure reduce churn probability.  
Decision threshold tuning plays a critical role in aligning model output with business priorities.

---

