# Customer-churn-Prediction

📌 Project Overview

This project analyzes customer churn using the Telco Customer Churn dataset and builds a machine learning classification model to predict whether a customer is likely to churn.

The project covers:

Data inspection and understanding

Data type conversion

Missing-value handling

Duplicate-value checking

Outlier detection and capping

Exploratory Data Analysis (EDA)

Categorical feature encoding

Feature/target separation

Train-test splitting

Feature standardization

Logistic Regression model training

Model evaluation using accuracy and a confusion matrix

Saving the trained model and preprocessing objects for future prediction/deployment

📊 Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains 7,043 customer records and 21 columns, including customer information, services, contract details, charges, and the churn target.

Important variables include:

gender

SeniorCitizen

Partner

Dependents

tenure

PhoneService

MultipleLines

InternetService

OnlineSecurity

OnlineBackup

DeviceProtection

TechSupport

StreamingTV

StreamingMovies

Contract

PaperlessBilling

PaymentMethod

MonthlyCharges

TotalCharges

Churn

customerID is removed before model training because it is an identifier rather than a predictive feature.

🔎 Data Preprocessing

The notebook performs the following preprocessing steps:

Converts TotalCharges from text to numeric values.

Handles missing TotalCharges values using the column mean.

Checks for duplicate records.

Checks for missing values.

Detects and caps outliers in:

tenure

MonthlyCharges

TotalCharges

Encodes categorical columns using LabelEncoder.

Separates the target (Churn) from the features.

Splits the data into training and testing sets using an 80/20 split.

Standardizes the feature values using StandardScaler.

📈 Exploratory Data Analysis

The notebook includes visual analysis of the churn data, including:

Churn distribution

Boxplot-based outlier checking

Outlier capping and verification

🤖 Machine Learning Model

A Logistic Regression classification model is trained to predict customer churn.

Train/Test Split

Training samples: 5,634

Testing samples: 1,409

Split: 80% training / 20% testing

Model Performance

Metric

Score

Training Accuracy

80.87%

Testing Accuracy

78.71%

A confusion matrix is also generated in the notebook to evaluate the model's classification performance.

The reported metrics are based on the results currently present in the Jupyter Notebook.

💾 Saved Model Files

The repository contains the following saved machine learning artifacts:

File

Purpose

churn_model.pkl

Trained Logistic Regression model

scaler.pkl

Fitted StandardScaler

encoders.pkl

Encoders used for categorical variables

feature_columns.pkl

Exact feature-column order expected by the model

These files are intended to support future prediction/deployment work.

📁 Project Structure

Customer-Churn-Analysis-Prediction/
│
├── Customer_Churn_Analysis_Prediction.ipynb
├── Telco-Customer-Churn.csv
├── churn_model.pkl
├── encoders.pkl
├── feature_columns.pkl
├── scaler.pkl
├── README.md
└── requirements.txt

🛠️ Technologies Used

Python

Jupyter Notebook

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Joblib

🚀 How to Run the Project

1. Clone the repository

git clone <YOUR-GITHUB-REPOSITORY-URL>
cd Customer-Churn-Analysis-Prediction

2. Install the required libraries

pip install -r requirements.txt

3. Open the notebook

jupyter notebook

Then open:

Customer_Churn_Analysis_Prediction.ipynb

4. Run the notebook

Run the cells from top to bottom to reproduce the data preprocessing, EDA, model training, evaluation, and model-artifact creation.

🎯 Project Objective

The objective of this project is to use customer information and service-related features to identify patterns in customer churn and build a machine learning model capable of predicting churn.

👤 Author

Piyush Srivastava
