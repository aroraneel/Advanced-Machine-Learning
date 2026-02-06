# Credit Card Default Prediction using Random Forest

## 📌 Overview
This project focuses on predicting whether a credit card customer will **default on their next payment** using a **Random Forest Classifier**.  
It uses the **UCI Credit Card Default Dataset** and applies supervised machine learning for binary classification.

The goal is to support financial institutions in identifying high-risk customers.

---

## 🎯 Objectives
- Load and explore the UCI Credit Card dataset  
- Perform preprocessing and feature separation  
- Train a **Random Forest Classification model**  
- Evaluate model performance using:
  - Accuracy Score  
  - Confusion Matrix  
  - Classification Report  

---

## 📁 Dataset Information
- Dataset: **UCI Credit Card Default Dataset**
- Records: ~30,000 customers  
- Features: Demographics + payment history + bill amounts  
- Target Variable:
  - `default.payment.next.month`
  - 1 = Default  
  - 0 = No Default  

---

## 🔍 Methodology

### 1. Data Loading & Exploration
- Read dataset using Pandas  
- Check dataset shape, columns, and statistics  
- Verify missing values  

### 2. Feature & Target Split
- Features (`X`) → All columns except target  
- Target (`y`) → Default payment indicator  

### 3. Train-Test Split
- 80% Training Data  
- 20% Testing Data  

### 4. Model Training
- Algorithm: **Random Forest Classifier**
- Model trained on customer financial behavior patterns  

### 5. Model Evaluation
Evaluation metrics include:
- **Accuracy Score**
- **Confusion Matrix Heatmap**
- **Precision, Recall, F1-score Report**

---

## 📊 Results & Insights
- Random Forest provides strong performance for default prediction  
- Confusion matrix highlights correct vs incorrect classifications  
- Classification report gives detailed evaluation metrics  

---

## 🛠️ Tools & Libraries
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 🚀 Applications
- Credit risk assessment  
- Loan approval systems  
- Banking decision support  
- Financial analytics  

---

## 👤 Author
**Neel Arora**  
BCA Undergraduate | Data Science & Machine Learning Enthusiast  

---
