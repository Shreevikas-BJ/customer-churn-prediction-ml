# Customer Churn Prediction ML

A machine learning project that predicts whether a telecom customer is likely to churn based on demographic details, account information, and service usage behavior.

This project demonstrates an end-to-end classification workflow, including data cleaning, exploratory data analysis, feature encoding, model training, and performance evaluation using Python and Scikit-learn.

---

## Overview

Customer churn is one of the most important business problems for subscription-based companies. Losing customers directly affects revenue, retention costs, and long-term growth.

The goal of this project is to build a machine learning model that can identify customers who are likely to leave the service. By analyzing customer attributes such as tenure, contract type, monthly charges, internet service, and payment method, the model helps businesses understand churn patterns and take proactive retention actions.

---

## Problem Statement

Telecom companies often have large customer bases with different usage patterns and subscription behaviors. The challenge is to identify which customers are at high risk of churn before they cancel their service.

This project answers:

- Which customer attributes are strongly related to churn?
- Can customer churn be predicted using historical customer data?
- How well does a classification model perform on unseen customer records?
- What insights can help improve customer retention strategies?

---

## Dataset

The project uses the Telco Customer Churn dataset.

The dataset includes customer-level information such as:

- Customer demographics
- Tenure and account details
- Internet and phone service subscriptions
- Contract type
- Payment method
- Monthly and total charges
- Churn status

Source: Kaggle - Telco Customer Churn

---

## Tech Stack

| Category | Tools / Libraries |
|---|---|
| Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Model | Logistic Regression |
| Evaluation | Confusion Matrix, Classification Report, Accuracy Score |

---

## Project Workflow

      Raw Customer Data
           ↓
      Data Cleaning
          ↓
      Exploratory Data Analysis
           ↓
      Feature Encoding
           ↓
      Train-Test Split
           ↓
      Model Training
           ↓
      Model Evaluation
           ↓
      Churn Prediction Insights


## Key Steps
**1. Data Loading**

The customer churn dataset is loaded using Pandas for analysis and preprocessing.

**2. Data Cleaning**

The cleaning process includes:

Handling missing or inconsistent values
Removing unnecessary columns such as customer ID
Converting numerical columns stored as text into proper numeric format
Preparing the target variable for classification
**3. Exploratory Data Analysis**

EDA is performed to understand:

Overall churn distribution
Relationship between churn and customer tenure
Effect of contract type on churn
Impact of monthly charges and services on churn behavior
Correlation between numerical variables

**4. Feature Encoding**

Since machine learning models require numerical input, categorical variables are converted into numerical format using encoding techniques.

**5. Model Building**

A Logistic Regression model is trained to classify customers into:

Churn
No Churn

**6. Model Evaluation**

The model is evaluated using:

Accuracy Score
Confusion Matrix
Precision
Recall
F1-Score
Classification Report
Example Business Use Case

A telecom company can use this model to identify customers who are likely to churn and take action before they leave.

Example retention actions:

Offer personalized discounts to high-risk customers
Improve support for customers with short tenure
Target month-to-month contract users with long-term plan incentives
Analyze payment method or service-related churn patterns

## Project Structure
customer-churn-prediction-ml/
│
├── Churn_Data.csv
├── customer_churn.py
└── README.md

## Getting Started

**1. Clone the repository**
git clone https://github.com/Shreevikas-BJ/customer-churn-prediction-ml.git
cd customer-churn-prediction-ml

**2. Create a virtual environment**
python -m venv venv

## Activate the environment:

Windows

venv\Scripts\activate

macOS / Linux

source venv/bin/activate

**3. Install dependencies**
pip install pandas numpy matplotlib seaborn scikit-learn

## Run the Project
python customer_churn.py

The script will load the dataset, clean the data, train the model, and display evaluation metrics.

## Sample Output
Accuracy Score: 0.80

Classification Report:
              precision    recall  f1-score   support

No Churn        0.84       0.90      0.87
Churn           0.65       0.52      0.58

Note: Actual results may vary depending on preprocessing, train-test split, and model configuration.

## Key Learnings

This project helped demonstrate:

How to approach a business classification problem
How to clean and prepare customer data for machine learning
How categorical variables affect model training
How to evaluate a classification model beyond accuracy
How churn prediction can support customer retention strategies
Future Improvements
Add advanced models such as Random Forest, XGBoost, or LightGBM
Perform hyperparameter tuning
Add feature importance analysis
Handle class imbalance using SMOTE or class weights
Build a Streamlit dashboard for interactive churn prediction
Deploy the model as an API using FastAPI
Add model explainability using SHAP
Author

**Shreevikas Bangalore Jagadish**
Graduate Student, Information Technology and Management
Illinois Institute of Technology

GitHub: Shreevikas-BJ
LinkedIn: shreevikasbj
Portfolio: datascienceportfol.io/shreevikasbj
Repository
https://github.com/Shreevikas-BJ/customer-churn-prediction-ml

One small suggestion: since this repo currently has only `Churn_Data.csv`, `customer_churn.py`, and `README.md`, keep the README simple and beginner-friendly like this. Later, when you add advanced models or a Streamlit app, we can upgrade the README to look more production-style.
::contentReference[oaicite:0]{index=0}
