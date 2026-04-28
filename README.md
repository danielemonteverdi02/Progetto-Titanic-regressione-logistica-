# 🚢 Titanic Survival Prediction – Logistic Regression

## 📌 Project Overview
This project focuses on the analysis and prediction of passenger survival on the Titanic using machine learning techniques.

The main objective is to build an accurate predictive model based on passenger characteristics and additional features obtained through feature engineering.

---

## 🎯 Objective
- Analyze the Titanic dataset
- Handle missing data effectively
- Engineer new informative features
- Build a predictive model using logistic regression
- Evaluate model performance on unseen data

---

## 🗂 Dataset
The dataset used is the official Titanic dataset from Kaggle, divided into:

- **Training set (train.csv)**: includes passenger information and survival outcome
- **Test set (test.csv)**: includes passenger features without survival labels

---

## 🔢 Variables

- **survival** → 0 = No, 1 = Yes  
- **pclass** → Ticket class (1 = First, 2 = Second, 3 = Third)  
- **sex** → Gender  
- **age** → Age (can be fractional if estimated)  
- **sibsp** → Number of siblings/spouses aboard  
- **parch** → Number of parents/children aboard  
- **ticket** → Ticket number  
- **fare** → Ticket price  
- **cabin** → Cabin number  
- **embarked** → Port of embarkation (C, Q, S)  

---

## 🧠 Methodology

### Data Preprocessing
- Data cleaning and anomaly handling
- Missing value imputation (single imputation and MICE)

### Feature Engineering
- Creation of new variables to improve model performance

### Encoding & Scaling
- One-hot encoding for categorical variables
- Scaling of numerical features

### Model
- Logistic Regression
- 10-fold Cross-Validation

### Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- ROC AUC

---

## 📊 Results

- **Cross-validation Accuracy**: 0.81 ± 0.04  
- **Precision**: 0.75 ± 0.07  
- **Recall**: 0.78 ± 0.03  
- **F1-score**: 0.76 ± 0.04  
- **ROC AUC**: 0.86 ± 0.03  

On the validation set:
- **Accuracy**: 0.79  

---

## 🚀 Conclusion
The model achieves solid performance both in cross-validation and on the validation set, showing good predictive capability and a balanced trade-off between precision and recall.

Possible improvements include:
- Testing more complex models
- Applying class balancing techniques
- Enhancing feature engineering
