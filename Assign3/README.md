# Assignment 3: Regression Analysis - Loan Sanction Prediction

## Institution
**Sri Sivasubramaniya Nadar College of Engineering, Chennai**  
**Subject**: UCS2612 – Machine Learning Algorithms Laboratory  

## 1. Aim and Objective
The objective of this assignment is to perform regression analysis to predict the **Loan Sanction Amount** based on various customer attributes. The experiment involves implementing and comparing the performance of multiple regression models:
- **Linear Regression**
- **Ridge Regression** (L2 Regularization)
- **Lasso Regression** (L1 Regularization)
- **Elastic Net Regression**

## 2. Dataset Description
The dataset consists of loan applicant details.
- **Files**: `train (2).csv`, `test.csv`
- **Target Variable**: `Loan Sanction Amount` (Continuous)
- **Features**:
  - **Categorical**: Customer ID, Name, Gender, Income Stability, Profession, Type of Employment, Location, Expense Type 1 & 2, Has Active Credit Card, Property Location.
  - **Numerical**: Age, Income (USD), Loan Amount Request (USD), Current Loan Expenses (USD), Credit Score, No. of Defaults, etc.

## 3. Workflow
The notebook (`ML3VSR.ipynb`) follows these steps:
1.  **Data Loading**: Reading train and test datasets.
2.  **Preprocessing**:
    -   Handling null values.
    -   Encoding categorical variables.
    -   Scaling numerical features.
3.  **Exploratory Data Analysis (EDA)**:
    -   Histograms and Boxplots for distribution and outlier detection.
    -   Correlation heatmaps to identify relationships between features.
4.  **Model Training**:
    -   Training Linear, Ridge, Lasso, and Elastic Net models.
5.  **Evaluation**:
    -   Comparing models using metrics such as **R² Score** and **Mean Squared Error (MSE)**.
