# Titanic Machine Learning Project

This repository contains my explorations of machine learning models on the **Titanic dataset**. The goal is to predict passenger survival using structured feature engineering, pipelines, and model evaluation. The project is ongoing — I plan to add more models, hyperparameter tuning, and performance analysis over time.  

---

## Current Implementations

### 1. Logistic Regression Pipeline
- **Preprocessing:**  
  - Impute missing numerical values with median  
  - Standardize numerical features (`Age`, `Fare`, `SibSp`, `Parch`, `FamilySize`, `IsAlone`)  
  - Impute missing categorical values with most frequent  
  - One-Hot Encode categorical features (`Sex`, `Embarked`, `Pclass`)  

- **Feature Engineering:**  
  - `FamilySize` = `SibSp` + `Parch` + 1  
  - `IsAlone` = 1 if passenger is alone, else 0  

- **Model:** Logistic Regression (`max_iter=1000`)  

- **Results (Current Run):**  
  - Train Accuracy: ~[Insert value]  
  - Test Accuracy: ~[Insert value]  

---

### 2. XGBoost Pipeline with Grid Search and Feature Importance
- **Upgraded from logistic regression:** Using **XGBoost** for better predictive power  
- **Hyperparameter Tuning:** GridSearchCV within a pipeline for `n_estimators`, `max_depth`, `learning_rate`, and `subsample`  
- **Feature Importance Analysis:**  
  - Extracted post-preprocessing importances  
  - Top contributors: `Sex`, `Title`, `FarePerPerson`  
  - Visualization included in the repository  

- **Notes:**  
  - Ensures **no data leakage**  
  - Correctly handles categorical features and pipeline transformations  


