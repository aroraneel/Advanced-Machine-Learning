# Adult Income Prediction using XGBoost Classifier

## 📌 Overview
This project predicts whether a person earns **more than $50K per year** based on demographic and employment-related features.

The model is built using **XGBoost (Extreme Gradient Boosting)**, a powerful machine learning algorithm widely used for structured/tabular classification problems.

The project includes preprocessing, categorical encoding, feature scaling, model training, and evaluation using classification metrics.

---

## 🎯 Objectives
- Analyze the Adult Census Income dataset  
- Encode categorical features into numeric form  
- Apply feature scaling for better performance  
- Train an XGBoost classification model  
- Predict income category (`<=50K` or `>50K`)  
- Evaluate results using:
  - Accuracy Score  
  - Confusion Matrix  
  - Classification Report  

---

## 📁 Dataset Information
- Dataset: **Adult Census Income Dataset**
- Target Variable:
  - `income`

### Classes:
- `<=50K` → Low Income  
- `>50K` → High Income  

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

### 1. Data Loading & Exploration
- Dataset loaded using Pandas  
- Shape, data types, missing values, and class distribution analyzed  

---

### 2. Categorical Feature Encoding
- Adult dataset contains multiple categorical columns  
- All categorical features are converted into numeric form using:
  - `LabelEncoder`

A mapping dictionary is also stored for reference.

---

### 3. Train-Test Split
- Dataset split into:
  - 80% Training  
  - 20% Testing  
- Random state fixed for reproducibility  

---

### 4. Feature Scaling
- Standardization applied using `StandardScaler`  
- Ensures features are on the same scale before training  

---

## 🚀 Model Development (XGBoost)

### Algorithm Used
- **XGBClassifier**

### Hyperparameters
- `n_estimators = 300`
- `learning_rate = 0.05`
- `max_depth = 5`
- `subsample = 0.8`
- `colsample_bytree = 0.8`

XGBoost improves performance through boosting and ensemble learning.

---

## 📊 Model Evaluation

### Metrics Used
- Accuracy Score  
- Confusion Matrix Heatmap  
- Precision, Recall, F1-score (Classification Report)

Visualization is done using Seaborn heatmaps.

---

## 🛠️ Tools & Libraries
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost  

---

## 🚀 Applications
- Income classification systems  
- Census-based economic analysis  
- HR and demographic analytics  
- Machine learning classification with boosting  

---

## 👤 Author
**Neel Arora**  
BCA Undergraduate | Data Science & Machine Learning Enthusiast  

---
