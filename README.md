# Telecom Customer Churn Prediction

## Project Overview
This project analyzes the Telco Customer Churn dataset and applies various machine learning algorithms to predict customer churn.  
Customer churn is when customers leave a service. Predicting churn helps telecom companies take action to retain valuable customers.

---

## Dataset
- Rows: 7043  
- Columns: 21  
- Target: `Churn` (Yes/No → converted to 1/0)  
- Features include:  
  - `gender`, `SeniorCitizen`, `Partner`, `Dependents`  
  - `tenure`, `PhoneService`, `InternetService`, `Contract`, etc.  
  - `MonthlyCharges`, `TotalCharges`  

---

## Steps Performed
### 1. Exploratory Data Analysis (EDA)
- Checked dataset info, missing values, distributions.  
- Visualized churn rates, tenure, monthly charges, and contract types.  

### 2. Data Cleaning
- Converted `TotalCharges` (object → float).  
- Handled missing values with mean/median imputation.  
- Dropped `customerID` (not useful for prediction).  
- Encoded categorical variables with Label Encoding.  

### 3. Correlation Matrix
- Plotted a heatmap for numerical columns (`tenure`, `MonthlyCharges`, `TotalCharges`).  
- Observed strong correlation between `tenure` and `TotalCharges`.  

### 4. Machine Learning Models
Implemented three models:
- Logistic Regression (baseline)  
- Support Vector Machine (SVM)  
- Decision Tree  

### 5. Model Evaluation
- Used accuracy, precision, recall, f1-score.  

## Results
- Logistic Regression → Balanced and reliable.  
- SVM → High accuracy, captures complex patterns.  
- Decision Tree → Easy to interpret but risk of overfitting.  

---

## Key Insights
- Customers with month-to-month contracts and high monthly charges are most likely to churn.  
- Long-tenure customers are less likely to leave.  
- Payment method also influences churn.  

---

## Business Recommendations
- Offer discounts or loyalty rewards to customers on month-to-month contracts.  
- Encourage long-term contracts (1-year or 2-year).  
- Monitor high-bill customers and provide special offers.  

---

## Tech Stack
- Python  
- Pandas, Numpy → Data Cleaning & Processing  
- Matplotlib, Seaborn → Data Visualization  
- Scikit-Learn → Machine Learning Models  


