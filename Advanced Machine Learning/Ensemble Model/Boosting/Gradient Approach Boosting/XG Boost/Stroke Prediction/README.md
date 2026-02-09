# Stroke Prediction using XGBoost Classifier

## 📌 Overview
This project predicts whether a patient is likely to suffer a **stroke** based on healthcare and lifestyle-related features.

The model is developed using **XGBoost Classifier**, a high-performance boosting algorithm widely used for medical risk prediction and classification tasks.

The workflow includes data cleaning, BMI missing value handling, categorical encoding, feature scaling, model training, evaluation, and feature importance visualization.

---

## 🎯 Objectives
- Analyze the Stroke Healthcare Dataset  
- Handle missing values and remove duplicate records  
- Convert categorical patient information into numeric form  
- Train an XGBoost model for stroke risk prediction  
- Evaluate model performance using classification metrics  
- Visualize important features contributing to stroke prediction  

---

## 📁 Dataset Information
- Dataset: **Healthcare Stroke Prediction Dataset**
- Target Variable:
  - `stroke`

### Classes:
- `0` → No Stroke  
- `1` → Stroke  

### Features Include:
- Gender  
- Age  
- Hypertension  
- Heart Disease  
- Marital Status  
- Work Type  
- Residence Type  
- Average Glucose Level  
- BMI  
- Smoking Status  

---

## 🔍 Methodology

### 1. Data Loading & Exploration
- Dataset loaded using Pandas  
- Checked dataset shape, columns, and data types  
- Removed duplicate rows for cleaner training  

---

### 2. Missing Value Handling
- BMI column contains missing values  
- Missing BMI values replaced using the most frequent value (mode)

---

### 3. Categorical Encoding
Many columns are categorical (gender, work type, smoking status, etc.)

All categorical features are converted into numeric form using:
- `LabelEncoder`

A mapping dictionary is also stored for reference.

---

### 4. Train-Test Split
- Dataset split into:
  - 80% Training  
  - 20% Testing  
- Random state fixed for reproducibility  

---

### 5. Feature Scaling
- Standardization applied using `StandardScaler`
- Ensures all features contribute equally to the model

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

XGBoost improves prediction performance through boosting and ensemble learning.

---

## 📊 Model Evaluation

### Metrics Used
- Accuracy Score  
- Confusion Matrix  
- Classification Report (Precision, Recall, F1-score)

A heatmap visualization is generated for the confusion matrix.

---

## 📌 Feature Importance
The project also includes a feature importance bar chart to highlight which health factors contribute most to stroke prediction.

This helps in understanding the medical risk indicators more clearly.

---

## 🛠️ Tools & Libraries
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- XGBoost  

---

## 🚀 Applications
- Healthcare risk prediction systems  
- Stroke prevention and early warning tools  
- Clinical decision support  
- Medical machine learning classification projects  

---

## 👤 Author
**Neel Arora**  
BCA Undergraduate | Data Science & Machine Learning Enthusiast  

---
