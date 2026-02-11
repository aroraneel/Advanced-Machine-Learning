# Income Prediction using CatBoost Classifier (Adult Census Dataset)

## 📌 Overview
This project predicts whether a person earns **more than $50K per year** using the well-known **Adult Census Income Dataset**.

The model is built using **CatBoost Classifier**, which is highly effective for datasets containing categorical features without requiring heavy preprocessing.

The workflow includes data cleaning, categorical feature handling, model training, ROC-AUC evaluation, confusion matrix analysis, and feature importance visualization.

---

## 🎯 Objectives
- Predict income category (`<=50K` or `>50K`)
- Handle categorical features automatically using CatBoost
- Train a high-performance boosting classifier
- Evaluate model performance using:
  - Accuracy
  - Confusion Matrix
  - Classification Report
  - ROC Curve & AUC Score
- Visualize top contributing features

---

## 📁 Dataset Information
- Dataset: **Adult Census Income Dataset**
- Target Column:
  - `income`

### Target Classes:
- `0` → Income ≤ 50K  
- `1` → Income > 50K  

### Features Include:
- Age  
- Workclass  
- Education  
- Marital Status  
- Occupation  
- Relationship  
- Race  
- Gender  
- Capital Gain / Loss  
- Hours per Week  
- Native Country  

---

## 🔍 Methodology

### 1. Data Loading & Cleaning
- Dataset loaded using Pandas  
- Duplicate records removed  
- Checked dataset shape, null values, and unique values

---

### 2. Target Encoding
The income column is converted into binary form:

- `<=50K → 0`
- `>50K → 1`

---

### 3. Categorical Feature Handling
CatBoost directly supports categorical features.

Categorical columns are automatically detected:

- Extracted using `object` datatype
- Passed into the model using feature indices

---

### 4. Train-Test Split
Dataset split into:

- 80% Training  
- 20% Testing  

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
- `class_weights = [1, 3]` (to handle imbalance)

CatBoost is especially powerful for structured/tabular datasets with mixed feature types.

---

## 📊 Model Evaluation

### Metrics Used
- Accuracy Score  
- Confusion Matrix  
- Classification Report  
- ROC Curve  
- AUC Score  

---

### ROC Curve & AUC
The project generates a full ROC curve and calculates the AUC score to measure classification quality.

A higher AUC indicates stronger separation between income classes.

---

## 📌 Feature Importance Analysis
The model extracts feature importance values and visualizes the **Top 5 most influential features** using a pie chart.

This helps interpret which attributes contribute most to predicting high income.

---

## 🛠️ Tools & Libraries
- Python  
- Pandas  
- CatBoost  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 🚀 Applications
- Income group prediction systems  
- Demographic-based financial analytics  
- Social and economic research  
- Tabular classification using boosting models  

---

## 👤 Author
**Neel Arora**  
BCA Undergraduate | Data Science & Machine Learning Enthusiast  

---
