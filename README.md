# Titanic Survival Prediction 🛳️

This project predicts whether a passenger survived the Titanic disaster using **Logistic Regression**.  
It is a beginner-friendly, end-to-end machine learning project built with **Python and Scikit-learn**.

---

## 📌 Project Overview

The goal of this project is to:
- Understand the full ML workflow
- Practice data preprocessing and feature engineering
- Train and evaluate a classification model
- Create a valid Kaggle submission

Dataset used: **Kaggle Titanic Dataset**

---

## 🧠 Machine Learning Approach

- **Model**: Logistic Regression  
- **Problem Type**: Binary Classification  
- **Evaluation**: 5-Fold Cross Validation (Accuracy)

---

## 🔧 Features Used

- Age (missing values filled with median)
- Sex (encoded: male = 0, female = 1)
- Fare (median imputation)
- Embarked (one-hot encoded)
- FamilySize = SibSp + Parch + 1
- IsAlone (binary feature)

Unused columns:
- Name
- Ticket
- Cabin

---

## 📊 Model Evaluation

- Cross-validation accuracy is used to estimate model performance
- This helps reduce overfitting and gives a more reliable accuracy estimate

