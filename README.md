# 📉 Customer Churn Prediction using Python and Tableau

## 🔍 Project Overview
This project focuses on predicting customer churn in a telecom company using machine learning techniques in Python, and visualizing business insights through interactive Tableau dashboards. The goal is to help stakeholders understand churn behavior and identify retention opportunities.

## 🚀 Problem Statement
Customer churn is a major concern for subscription-based businesses. Reducing churn is often more cost-effective than acquiring new customers. The objective of this project is to:
- Predict which customers are likely to churn.
- Understand key drivers behind customer churn using visual analysis.

## 🧰 Tools & Technologies
- **Python**: Data Cleaning, EDA, Feature Engineering, Model Building
- **Pandas, NumPy, Matplotlib, Seaborn**: Data manipulation and visualization
- **Scikit-learn**: Machine Learning (Logistic Regression, Random Forest, etc.)
- **Tableau**: Interactive Dashboards
- **Jupyter Notebook**: For code development
- **CSV Dataset**: Provided by the telecom company

## 📁 Project Structure
customer-churn-prediction
-├── data/
-│ └── churn_data.csv
-├── cleaned_data/
-│ └── churn_cleaned.csv
-├── notebooks/
-│ └── churn_modeling.ipynb
-├── dashboard/
-│ └── churn_dashboard.twbx
-├── images/
-│ └── churn_dashboard_screenshot.png
-├── README.md
-└── requirements.txt

## Python Code
<a href="https://github.com/Shreyathudi-217/Customer-Churn-Prediction/blob/main/Customer%20Churn%20Prediction%20.ipynb">python code

## 📊 Tableau Dashboard
The Tableau dashboard provides interactive insights on:
- Churn rate by contract type, internet service, gender, etc.
- Tenure, MonthlyCharges, and TotalCharges comparisons by churn
- Filter controls for `Gender`, `Contract`, `PaymentMethod`, and `SeniorCitizen`
<a href="https://public.tableau.com/app/profile/shreya.thudi/viz/CustomerChurnPrediction_17525698809110/Dashboard1">Tableau dashboard

## 📈 Machine Learning Workflow
1. **Data Preprocessing**
   - Removed nulls and inconsistencies
   - Converted categorical columns using Label Encoding and OneHotEncoding
   - Saved cleaned data for modeling and Tableau

2. **Exploratory Data Analysis**
   - Used Seaborn and Matplotlib to find correlations
   - Churn patterns observed across services and demographics

3. **Model Training**
   - Trained models: Logistic Regression, Random Forest, Decision Tree
   - Evaluated using Accuracy, Precision, Recall, F1-Score

4. **Best Performing Model**
   - Model: *Random Forest Classifier*
   - Accuracy: *~80%*
   - Feature importance: `Contract`, `tenure`, `MonthlyCharges`

## 📌 Key Insights
- **Month-to-month** contract customers churn the most
- Customers with **high MonthlyCharges and low tenure** are more likely to churn
- **Fiber optic** internet users show higher churn than DSL
- **Long-term contracts** reduce churn

## 📂 Dataset Info
The dataset contains ~7,000 records and 20+ features including:
- `customerID`, `gender`, `SeniorCitizen`, `Partner`, `tenure`
- `PhoneService`, `MultipleLines`, `InternetService`, `PaymentMethod`
- `MonthlyCharges`, `TotalCharges`, `Churn`
> 📌 Source: [Kaggle - Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

## 🧠 Future Improvements
- Use advanced models (XGBoost, LSTM for time series churn)
- Integrate model prediction directly into Tableau using Python Tableau Server Client
- Implement customer retention recommendation system


