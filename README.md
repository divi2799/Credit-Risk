# Project Report: Credit Risk Analytics (XGBoost, Azure ML)

## 1. Introduction
Financial institutions need reliable systems to evaluate customer creditworthiness and minimize loan defaults.  
This project focused on building a **credit risk classification model** using XGBoost on **Azure ML pipelines**, with explainability and automated monitoring, ensuring high accuracy and business usability.

---

## 2. Objectives
- Analyze customer demographics, transactions, and repayment history.  
- Engineer meaningful financial features to improve model accuracy.  
- Train and tune an **XGBoost classifier** using Azure ML Studio pipelines.  
- Deploy automated pipelines for model retraining and drift detection.  
- Provide **interpretable results** with SHAP values to aid business stakeholders.  

---

## 3. System Architecture
1. **Data Ingestion:** Customer demographics, transaction history, credit scores, repayment behavior.  
2. **Feature Engineering:** Derived debt-to-income ratio, credit utilization, repayment patterns.  
3. **Model Training (XGBoost):** Hyperparameter tuning for maximum performance.  
4. **Deployment:** Automated pipelines in Azure ML for monitoring and retraining.  
5. **Explainability:** SHAP values for decision drivers (missed payments, history length).  

---

## 4. Implementation
- Conducted **EDA** to detect anomalies and handle missing values.  
- Engineered domain-specific features:  
  - **Debt-to-Income Ratio** – ratio of total debt to income.  
  - **Credit Utilization** – proportion of credit limit used.  
  - **Repayment Behavior** – history of on-time vs late payments.  
- Trained **XGBoost classifier** with cross-validation.  
- Hyperparameter tuning (learning rate, max depth, n_estimators) done in **Azure ML pipelines**.  
- Deployed pipelines for **drift monitoring** and **automated retraining** with fresh data.  
- Applied **SHAP values** for feature attribution and business interpretability.  

---

## 5. Results
- Increased **AUC from 0.84 → 0.92** (+8% over baseline).  
- Maintained **production accuracy above 90%** through retraining.  
- Reduced loan default rates by **5%** via targeted interventions.  
- Business stakeholders gained visibility into key drivers (late payments, utilization).  

---

## 6. Future Enhancements
- Integrate alternative data sources (social data, transaction metadata).  
- Explore ensemble approaches combining XGBoost and neural networks.  
- Extend deployment with real-time scoring APIs.  
