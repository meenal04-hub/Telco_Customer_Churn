# 📊 Telco Customer Churn Prediction

## 🔹 Introduction
Customer churn refers to the loss of clients or subscribers who discontinue their services.  
For telecom companies, predicting churn is crucial for improving customer retention and reducing revenue losses.  
This project analyzes customer behavior and builds machine learning models to predict churn with high accuracy.

---

## 🔹 Problem Statement
The challenge is to accurately identify which customers are likely to churn based on demographic, usage, and billing information.  

Objectives:
1. Perform **exploratory data analysis (EDA)** to understand churn patterns.  
2. Build classification models to predict customer churn.  
3. Compare models based on accuracy, precision, recall, and F1-score.  
4. Derive business insights to help improve retention strategies.  

---

## 🔹 Dataset
The dataset contains information about telecom customers including:  
- **Demographics**: Gender, Senior Citizen, Partner, Dependents  
- **Services**: Phone service, Internet service, Streaming services, Contract type  
- **Billing**: Monthly Charges, Total Charges, Payment Method  
- **Target Variable**: `Churn` (Yes/No)  

---

## 🔹 Methodology

### 1. Data Preprocessing
- Checked and handled missing values.  
- Converted categorical features into numerical values using encoding.  
- Scaled continuous features like `MonthlyCharges`, `TotalCharges`, and `Tenure`.  

### 2. Exploratory Data Analysis (EDA)
- Distribution of churn vs. non-churn customers.  
- Relationship between contract type, monthly charges, and churn.  
- Identified customer segments with higher churn risk.  

🔑 **Key Findings from EDA**:
- Customers with **month-to-month contracts** had the highest churn rate.  
- Customers with **higher monthly charges** were more likely to churn.  
- **Senior citizens** and customers without partners/dependents had a higher churn probability.  
- Long-term contracts significantly reduced churn.  

### 3. Modeling
Implemented multiple machine learning algorithms:  
- Logistic Regression  
- Random Forest Classifier  
- XGBoost Classifier  

### 4. Evaluation
Models were evaluated using:  
- Accuracy  
- Precision, Recall, and F1-score  
- ROC-AUC score  

---

## 🔹 Results & Insights
- **Logistic Regression**: Good baseline, interpretable but lower recall.  
- **Random Forest**: Strong balance of precision and recall, performed well.  
- **XGBoost**: Best performing model with the highest ROC-AUC score.  

📌 **Business Insights**:
- Retention strategies should focus on **customers with monthly contracts & high charges**.  
- Offering **discounts, bundled services, or long-term contracts** can help reduce churn.  
- Targeted campaigns for **senior citizens and single customers** can improve retention.  

---

## 🔹 Conclusion
- Machine learning models can effectively predict churn and help telecom companies take proactive measures.  
- **XGBoost** was the most effective model.  
- Business interventions like **loyalty programs and contract-based offers** can reduce churn.  

---

## 🔹 Future Enhancements
- Hyperparameter tuning to further improve accuracy.  
- Use SHAP values or feature importance for explainability.  
- Develop a **real-time churn prediction dashboard**.  

---
