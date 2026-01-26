# Assignment 2: Naive Bayes and KNN Classification

**Student:** Rahul V S (3122235001104)

## Overview
This assignment implements and evaluates Naive Bayes and K-Nearest Neighbors (KNN) algorithms for a classification task (Spam Detection).

## Files
- `ML_Assign2_VSR.ipynb`: The main Jupyter notebook.
- `spambase_csv_Kaggle.csv`: The dataset used for training and testing.

## Methodology

### 1. Data Preprocessing
- Imported `spambase_csv_Kaggle.csv`.
- Performed train-test split.
- Standardized features using `StandardScaler` for KNN (distance-based) and Gaussian Naive Bayes.

### 2. Models Implemented
- **Naive Bayes**:
    - `GaussianNB`: For continuous features assuming normal distribution.
    - `MultinomialNB`: For discrete counts.
    - `BernoulliNB`: For binary/boolean features.
- **K-Nearest Neighbors (KNN)**:
    - Trained `KNeighborsClassifier`.
    - Analyzed the effect of `k` (neighbors) on accuracy (Accuracy vs. K plot).

### 3. Evaluation Metrics
The models were evaluated using the following metrics:
- **Accuracy Score**
- **Precision, Recall, F1-Score**
- **Confusion Matrix**
- **ROC Curve and AUC**: Compared the performance of different Naive Bayes variants.

## Results
- **Naive Bayes**: Comparison of AUC scores for Gaussian, Multinomial, and Bernoulli classifiers.
- **KNN**: Optimization of `k` value for the best classification accuracy.

## How to Run
1.  Install dependencies: `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`.
2.  Open `ML_Assign2_VSR.ipynb`.
3.  Run all cells to see the training process and evaluation plots.
