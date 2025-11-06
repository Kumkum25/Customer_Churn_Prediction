# 📉 Customer Churn Prediction

## 📖 Overview  
This project focuses on predicting whether a customer will churn (i.e., stop being a customer) using machine learning techniques. The goal is to help businesses identify at-risk customers early so they can take proactive steps to retain them.

---

## 🎯 Objective  
To develop and evaluate a set of machine learning models that predict customer churn based on customer demographics, service usage, account information, and other behavioural factors.

---

## 📊 Dataset Description  
The dataset contains a variety of features capturing customer account information, usage patterns, services subscribed, and churn status.  
*(Exact column names and counts are available in the notebook.)*

Key types of features include:  
- Customer identifiers and account information  
- Demographics (age, gender, etc.)  
- Service and product usage features  
- Billing and payment method features  
- Tenure, monthly charges, total charges  
- Churn label (target variable)  

---

## ⚙️ Data Preprocessing & Feature Engineering  
- Handled missing values and converted data types appropriately  
- Created derived features such as tenure buckets, service counts, payment method flags  
- Encoded categorical variables (One-Hot / Label Encoding)  
- Scaled or normalized numerical features as needed  
- Split data into training and testing sets with an appropriate random state  
- Addressed class imbalance (if present) using oversampling / undersampling / class weights  

---

## 🔍 Exploratory Data Analysis (EDA)  
- Visualized distributions of churn vs. non-churn customers  
- Examined relationships between features (e.g., tenure, monthly charges, services) and churn  
- Generated correlation heatmaps and feature importance previews  
- Identified key distinguishing patterns for churners  

---

## 🤖 Model Development  
Trained and compared multiple classification models:  
- **Logistic Regression**  
- **Random Forest Classifier**  
- **Gradient Boosting Classifier**  
- **XGBoost Classifier**  
- **CatBoost Classifier**  

---

## 📈 Model Evaluation  
Evaluated models using classification metrics:  
- **Accuracy**  
- **Precision**  
- **Recall**  
- **F1 Score**  
- **ROC-AUC Score**  

Selected the best model based on a balanced performance across these metrics and its ability to generalize.

---

## 🧠 Key Insights  
- Some features (e.g., tenure, monthly charges, number of services) were strong predictors of churn.  
- Customers with shorter tenure, higher monthly charges, or fewer services were more likely to churn.  
- Proper feature engineering and handling of class imbalance significantly improved model performance.

---

## 🧰 Tools & Technologies Used  
- **Python**  
- **Pandas**, **NumPy**  
- **Matplotlib**, **Seaborn**  
- **Scikit-learn**  
- **XGBoost**, **CatBoost**  
- **Jupyter Notebook**

---

## 📁 Project Structure  
