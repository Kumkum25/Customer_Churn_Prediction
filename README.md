# 📉 Customer Churn Prediction

## 📖 Overview  
This project aims to predict **customer churn** — that is, whether a customer is likely to discontinue a service — using machine learning techniques.  
The analysis helps businesses, especially in the telecom sector, identify customers at risk of leaving so that proactive retention strategies can be implemented.

---

## 🎯 Objective  
To build and evaluate machine learning models that can predict customer churn based on service usage patterns, demographic data, and account information.

---

## 🧾 Dataset Description  
The dataset contains information about **7,043 customers** and **21 features** describing their demographics, subscription details, and service usage patterns.

### 📋 Columns Overview
| Feature | Description |
|----------|-------------|
| `customerID` | Unique ID assigned to each customer |
| `gender` | Gender of the customer (Male/Female) |
| `SeniorCitizen` | Indicates if the customer is a senior citizen (1 = Yes, 0 = No) |
| `Partner` | Whether the customer has a partner (Yes/No) |
| `Dependents` | Whether the customer has dependents (Yes/No) |
| `tenure` | Number of months the customer has stayed with the company |
| `PhoneService` | Whether the customer has a phone service |
| `MultipleLines` | If the customer has multiple lines |
| `InternetService` | Type of internet service (DSL/Fiber optic/None) |
| `OnlineSecurity` | Whether the customer has online security service |
| `OnlineBackup` | Whether the customer has online backup service |
| `DeviceProtection` | Whether the customer has device protection plan |
| `TechSupport` | Whether the customer has tech support |
| `StreamingTV` | Whether the customer has streaming TV service |
| `StreamingMovies` | Whether the customer has streaming movie service |
| `Contract` | Type of contract (Month-to-month, One year, Two year) |
| `PaperlessBilling` | Whether the customer uses paperless billing |
| `PaymentMethod` | Payment method used by the customer |
| `MonthlyCharges` | Monthly charges paid by the customer |
| `TotalCharges` | Total charges paid by the customer |
| `Churn` | Target variable (Yes = churned, No = retained) |

---

## ⚙️ Data Preprocessing & Cleaning  
- Handled missing values (notably in `TotalCharges`)  
- Converted categorical features into numerical form using **Label Encoding** and **One-Hot Encoding**  
- Normalized numeric variables for consistent scale  
- Split the dataset into **training** and **testing** sets  
- Ensured balanced class distribution where necessary  

---

## 🔍 Exploratory Data Analysis (EDA)  
- Visualized churn distribution to understand imbalance  
- Analyzed relationships between churn and key features such as `Contract`, `tenure`, `MonthlyCharges`, and `PaymentMethod`  
- Examined correlations among numeric variables  
- Identified top factors influencing churn using visual insights  

---

## 🤖 Model Development  
Trained and compared multiple machine learning models, including:  
- **Logistic Regression**  
- **Random Forest Classifier**  
- **Gradient Boosting Classifier**  
- **XGBoost Classifier**  
- **CatBoost Classifier**

---

## 📈 Model Evaluation  
Evaluated model performance using the following metrics:  
- **Accuracy**  
- **Precision**  
- **Recall**  
- **F1 Score**  
- **ROC-AUC Score**

The final model was chosen based on a balanced trade-off between accuracy and recall, ensuring it effectively captures churned customers.

---

## 💡 Key Insights  
- Customers on **month-to-month contracts** and **paperless billing** tend to churn more.  
- Higher **MonthlyCharges** are linked with higher churn rates.  
- Long-term customers (`tenure` > 1 year) are significantly less likely to churn.  
- Providing additional services (like **OnlineSecurity**, **TechSupport**) reduces churn risk.  

---

## 🧰 Tools & Technologies Used  
- **Python**  
- **Pandas**, **NumPy**  
- **Matplotlib**, **Seaborn**  
- **Scikit-learn**  
- **XGBoost**, **CatBoost**  
- **Jupyter Notebook**

---
