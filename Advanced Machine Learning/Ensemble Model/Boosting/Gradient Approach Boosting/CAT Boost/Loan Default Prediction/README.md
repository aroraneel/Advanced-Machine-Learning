# Loan Default Prediction using CatBoost Classifier

## 📌 Overview
This project predicts whether a loan borrower will **fully repay the loan or default** using a supervised machine learning approach.

A **CatBoost Classifier** is implemented to handle both numerical and categorical features efficiently, providing strong performance on structured financial datasets.

The project includes full workflow: data exploration, visualization, model training, evaluation with ROC-AUC, and feature importance analysis.

---

## 🎯 Objectives
- Predict loan repayment status (`not.fully.paid`)
- Handle categorical loan purpose feature automatically
- Train a boosting-based classification model (CatBoost)
- Evaluate performance using:
  - Accuracy Score
  - ROC Curve & AUC Score
  - Confusion Matrix
  - Classification Report
- Visualize feature importance and loss curves

---

## 📁 Dataset Information
- Dataset: **Loan Data**
- Target Column:
  - `not.fully.paid`

### Target Classes:
- `0` → Loan Fully Paid  
- `1` → Loan Not Fully Paid (Default Risk)

### Key Features Include:
- Credit policy score  
- Interest rate  
- Installment amount  
- Annual income  
- Debt-to-income ratio  
- FICO score  
- Loan purpose (categorical)  

---

## 🔍 Methodology

### 1. Data Loading & Exploration
- Loaded dataset using Pandas  
- Displayed column info and dataset structure  
- Checked feature types and missing values  

---

### 2. Data Visualization

#### Target Class Distribution
A countplot is used to analyze class imbalance:

- More fully paid loans than defaults

#### Feature Correlation Heatmap
A correlation heatmap is generated to understand relationships between numerical features.

---

### 3. Feature Selection

- Target variable: `not.fully.paid`
- Input features: All remaining columns
- Categorical feature:
  - `purpose`

CatBoost directly supports categorical variables without manual encoding.

---

### 4. Train-Test Split
Dataset split into:

- 90% Training  
- 10% Testing  

Stratified sampling ensures balanced class distribution.

---

## 🚀 Model Development (CatBoost)

### Algorithm Used
- **CatBoostClassifier**

### Hyperparameters
- `iterations = 500`
- `learning_rate = 0.05`
- `depth = 6`
- `eval_metric = AUC`
- `class_weights = [1, 3]`
- `use_best_model = True`

Class weights help handle default-class imbalance effectively.

---

## 📊 Model Evaluation

### Metrics Used
- Accuracy Score  
- ROC-AUC Score  
- Confusion Matrix  
- Classification Report  

---

### Threshold-Based Prediction
Instead of the default threshold (0.5), a custom threshold is applied:

- `threshold = 0.4`

This improves sensitivity toward default detection.

---

### ROC Curve & AUC Score
The ROC curve is plotted to visualize model performance across thresholds.

A higher AUC indicates stronger classification ability.

---

## 📌 Feature Importance Analysis
The project extracts feature importance scores from CatBoost and visualizes them using a bar chart.

This helps identify the most influential financial factors affecting loan repayment.

---

## 📉 Training vs Validation Loss Curve
A loss curve is plotted to monitor:

- Model learning progress  
- Overfitting or underfitting trends  

Train and validation logloss curves provide training transparency.

---

## 🛠️ Tools & Libraries
- Python  
- Pandas, NumPy  
- CatBoost  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 🚀 Applications
- Loan default risk assessment  
- Credit scoring systems  
- Banking and finance decision support  
- Automated borrower risk classification  

---

## 👤 Author
**Neel Arora**  
BCA Undergraduate | Data Science & Machine Learning Enthusiast  

---