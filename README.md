<h1 align="center"> CSE445 (Machine Learning): Project </h1>
<h2 align="center"> Machine Learning-Based Phishing URL Detection
<p align="center">
 <img alt="Languages" src="https://img.shields.io/github/languages/count/haiderCho/CSE445-Project-MLPUD">
 <img alt="Repository size" src="https://img.shields.io/github/repo-size/haiderCho/CSE445-Project-MLPUD">
 <img alt="Contributors" src="https://img.shields.io/github/contributors/haiderCho/CSE445-Project-MLPUD">
 <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/haiderCho/CSE445-Project-MLPUD">
</p>
</h2>

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

This project presents a comprehensive machine learning pipeline to classify phishing URLs using multiple classifiers, data preprocessing techniques, and evaluation metrics.

## 📂 Project Overview

The pipeline involves:

- Fetching and preparing the dataset using the `ucimlrepo` package.
- Addressing class imbalance with techniques like **SMOTE**, **ADASYN**, and **Borderline SMOTE**.
- Feature selection using `SelectKBest` with ANOVA F-test.
- Model training with multiple classifiers: 
	- **Random Forest**, 
	- **SVM**, 
	- **Logistic Regression**, 
	- **Decision Trees**, 
	- **XGBoost**, 
	- **KNN**, 
	- **Gradient Boosting**, 
	- **StackingClassifier** (ensemble of multiple base learners).
- Evaluation using:
  - Accuracy
  - ROC AUC
  - Confusion matrix
  - Classification report
- Model interpretability with **LIME**.

## 🧰 Tools & Libraries

- **Python 3.x**
- pandas, numpy
- seaborn, matplotlib
- scikit-learn
- imbalanced-learn
- xgboost
- lime
- ucimlrepo

## 📈 Model Pipeline

1. **Data Loading** from UCI repository
2. **Data Preprocessing**:
   - Label encoding
   - Scaling
3. **Class Balancing**:
   - SMOTE, ADASYN, BorderlineSMOTE
4. **Feature Selection**:
   - `SelectKBest(f_classif)`
5. **Model Training**:
   - RandomForest, SVM, LogisticRegression, etc.
6. **Evaluation**:
   - Metrics + LIME explanations
