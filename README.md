# 📊 Telco Customer Churn Prediction

## 🔎 Project Overview
This project builds a **customer churn prediction system** for a telecom company using the [Telco Customer Churn dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn).  

Churn (Yes/No) represents whether a customer **left the company**. Predicting churn is critical since retaining customers is much more cost-effective than acquiring new ones.  

---

## 📂 Dataset Information
- **Source**: Kaggle – Telco Customer Churn  
- **Size**: 7,043 customers, 21 features  
- **Target Variable**: `Churn` (Yes / No)  

### Feature Categories
- **Demographics**: `gender`, `SeniorCitizen`, `Partner`, `Dependents`  
- **Services**: `PhoneService`, `InternetService`, `OnlineSecurity`, `StreamingTV`, etc.  
- **Financial**: `MonthlyCharges`, `TotalCharges`, `PaymentMethod`  

---

## 🛠️ Workflow
1. **Data Assessment**
   - Data quality check (types, missing values, inconsistencies)
   - Target variable analysis (churn rate & class imbalance)

2. **EDA**
   - Outlier detection (IQR + boxplots)
   - Univariate, bivariate & multivariate analysis
   - Churn patterns across demographics, services, and financial features  

3. **Feature Engineering**
   - `TenureCategory` (New / Established / Loyal)  
   - `ServiceCount` (number of services subscribed)  
   - `BundleUser` (both Internet + Phone)  
   - `ChargeCategory` (low / medium / high spenders)  

4. **Preprocessing & Transformations**
   - Missing value imputation (`TotalCharges → 0 for tenure=0`)  
   - Log + scaling transformations for skewed numeric features  
   - One-hot encoding for categorical features  

5. **Modeling**
   - Baseline: Logistic Regression, Decision Tree  
   - Ensemble methods: Random Forest, XGBoost, CatBoost  
   - Pipeline integration with preprocessing  

6. **Evaluation**
   - Metrics for imbalanced data: Precision, Recall, F1-score, ROC-AUC  
   - Performance comparison of models  

7. **Business Insights**
   - High-risk churn profiles  
   - Retention strategy recommendations  
   - Estimated revenue impact from reducing churn  

---

## ⚙️ Setup & Installation
Clone the repository:
```bash
git clone https://github.com/your-username/telco-churn-prediction.git
cd telco-churn-prediction
