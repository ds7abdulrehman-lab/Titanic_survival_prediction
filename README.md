# 🚢 Titanic Survival Prediction — End-to-End Machine Learning Pipeline

This project presents a **complete machine learning workflow** for predicting passenger survival on the Titanic dataset.

The goal of this project is to demonstrate **clean ML pipelines, feature engineering, model evaluation, and explainability**, following industry-aligned data science practices.

The workflow progresses from **baseline modeling to advanced model interpretability using SHAP**.

---

## 📂 Project Structure

This repository explores multiple modeling approaches for the Titanic survival prediction problem.

### ⭐ Main Notebook
**Titanic_Survival_Final_Model.ipynb**

Complete end-to-end pipeline including:

- Data preprocessing
- Feature engineering
- Model training
- Hyperparameter tuning
- Model evaluation
- SHAP explainability

This notebook represents the **final machine learning workflow**.

### Additional Experiments

**Logistic_reg_pipeline.ipynb**

Baseline model using Logistic Regression to establish benchmark performance.

**GridSearch_Pipeline.ipynb**

Hyperparameter tuning using GridSearchCV to optimize model performance.

**SHAP_Advance_Concept.ipynb**

Model interpretability using SHAP to understand feature contributions and prediction behavior.

---

## 🎯 Project Objectives

- Build **reproducible machine learning pipelines**
- Prevent **data leakage using Scikit-learn pipelines**
- Apply structured **feature engineering**
- Compare baseline and advanced models
- Perform **robust model evaluation**
- Interpret model predictions using **SHAP explainability**

---

## 📊 Dataset

Source: **Kaggle Titanic Dataset**

Target variable:

**Survived**
- `0` → Passenger did not survive  
- `1` → Passenger survived

Key features include:

- Passenger class
- Age
- Fare
- Gender
- Family relationships
- Port of embarkation

---

## ⚙️ Feature Engineering

Several custom features were created to improve predictive performance.

**IsAlone**

Binary indicator showing whether the passenger traveled alone.

**FarePerPerson**


**Title Extraction**

Passenger titles were extracted from names and rare titles were grouped together.


All transformations are implemented **inside Scikit-learn pipelines** to prevent data leakage.

---

## 🔧 Data Preprocessing

Implemented using **ColumnTransformer**.

### Numerical Features
- Median imputation
- Standard scaling

### Categorical Features
- Most frequent imputation
- One-hot encoding

All preprocessing steps are integrated directly into the machine learning pipeline.

---

## 🤖 Models Implemented

### Logistic Regression (Baseline Model)

- Used as a benchmark model
- Max iterations set to 1000
- Provides interpretable baseline results

---

### XGBoost Classifier (Final Model)

Used as the **final optimized model**.

Key characteristics:

- Integrated within a machine learning pipeline
- Hyperparameter tuning using **GridSearchCV**
- Optimized using **5-fold cross validation**
- Primary evaluation metric: **ROC-AUC**

Tuned parameters include:

- `n_estimators`
- `max_depth`
- `learning_rate`
- `subsample`
- `colsample_bytree`

---

## 📈 Model Evaluation

Evaluation goes beyond simple accuracy to understand model behavior:

- **ROC-AUC Score**
- **Confusion Matrix**
- **Classification Report**
- Precision
- Recall
- F1-Score
- **Precision–Recall Curve**
- **Learning Curves**

These metrics help evaluate both **model accuracy and generalization capability**.

---

## 🔍 Model Explainability (SHAP)

To understand how the model makes predictions, **SHAP (SHapley Additive exPlanations)** was applied.

### Global Explainability

SHAP summary plots highlight the most influential features:

- Age
- FarePerPerson
- FamilySize
- Passenger class features

### Local Explainability

SHAP waterfall plots explain individual passenger predictions, showing how each feature influences the final prediction.

This improves **model transparency and trust**.

---

## 🧠 Key Learnings

- Feature engineering can significantly improve model performance
- Machine learning pipelines prevent data leakage
- Evaluation metrics must go beyond simple accuracy
- Model explainability is critical for real-world ML applications

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- SHAP

---

## 📌 Project Status

**Completed**

Future improvements may include:

- Testing additional ensemble models
- Additional feature engineering
- Validation on external datasets

---

## 👨‍💻 Author

**Abdul Rehman**

Master’s Student — International Data Science  
Rome Business School

Actively seeking **Data Science / Machine Learning internship opportunities**

📧 ds.7abdulrehman@gmail.com
