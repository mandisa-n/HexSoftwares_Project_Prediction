# Loan Eligibility Prediction

This project is part of my **Week 1 internship at Hexsoft**. It focuses on predicting loan eligibility using machine learning classification techniques.

## Project Overview
The goal of this project is to predict whether a loan will be approved based on applicant information such as income, employment, credit history, and property area.

## Dataset
The dataset contains **614 records** with the following features:

- **Loan_ID** – Unique loan identifier (Object)  
- **Gender** – Male/Female (Object)  
- **Married** – Marital status (Object)  
- **Dependents** – Number of dependents (Object)  
- **Education** – Education level (Object)  
- **Self_Employed** – Self-employed or not (Object)  
- **ApplicantIncome** – Applicant monthly income (int64)  
- **CoapplicantIncome** – Co-applicant monthly income (float64)  
- **LoanAmount** – Loan amount in thousands (float64)  
- **Loan_Amount_Term** – Term of loan in months (float64)  
- **Credit_History** – 1 = meets guidelines, 0 = does not (float64)  
- **Property_Area** – Urban / Semiurban / Rural (Object)  
- **Loan_Status** – Loan approved or not (Y/N) – **Target variable** (Object)  

## Data Cleaning & Preprocessing
- **Handled missing values**:  
  - Categorical: Mode imputation  
  - Numerical: Mean imputation  
- Converted categorical variables using **One-Hot Encoding**  
- Combined **ApplicantIncome** and **CoapplicantIncome** into **TotalIncome**  
- Handled outliers by applying **log transformation** to numerical features  
- Scaled features using **StandardScaler**  
- Split data into training and testing sets  

## Modeling
Three classifiers were used to predict loan eligibility:

- **Decision Tree Classifier** – Accuracy: 72%  
- **Naive Bayes** – Accuracy: 83%  
- **Logistic Regression** – Accuracy: 84%  

## Key Learnings
- Data cleaning and preprocessing are crucial for accurate predictions.  
- Feature engineering, like combining income variables, can improve model performance.  
- Comparing different classifiers helps in selecting the best-performing model.
