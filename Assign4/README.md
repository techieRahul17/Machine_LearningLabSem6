# Assignment 4: Binary Classification using Linear and Kernel-Based Models

## Institution
**Sri Sivasubramaniya Nadar College of Engineering, Chennai**  
**Subject**: UCS2612 – Machine Learning Algorithms Laboratory  

## 1. Aim and Objective
The goal of this experiment is to classify emails as **Spam** or **Ham** (non-spam) using supervised learning classification algorithms. The project focuses on:
-   **Logistic Regression**
-   **Support Vector Machine (SVM)** (utilizing Linear, Polynomial, RBF, and Sigmoid kernels)
-   Hyperparameter tuning using **Grid Search**.
-   Analysis of regularization techniques.

## 2. Dataset Description
-   **Dataset**: Spambase
-   **File**: `spambase_csv.csv`
-   **Features**: 57 numerical attributes representing:
    -   Word frequencies (e.g., `word_freq_make`, `word_freq_money`).
    -   Character frequencies (e.g., `char_freq_$`, `char_freq_!`).
    -   Capital run lengths (average, longest, total).
-   **Target Variable**: `Class` (1 = Spam, 0 = Ham)

## 3. Workflow
The notebook (`ML4VSR.ipynb`) follows these steps:
1.  **Data Loading & Overview**: Examining dataset structure and statistics.
2.  **Preprocessing**:
    -   Checking for missing values.
    -   **StandardScaler** for simple feature scaling.
3.  **Exploratory Data Analysis (EDA)**:
    -   Visualizing class balance.
    -   Feature distribution plots.
4.  **Model Implementation & Tuning**:
    -   **Logistic Regression**: Analyzing the impact of regularization.
    -   **SVM**: Testing different kernels and tuning `C`, `gamma`, and `degree` parameters using GridSearchCV.
5.  **Evaluation**:
    -   Metrics: Accuracy, Precision, Recall, F1-Score.
    -   Classification Reports for detailed performance analysis.
