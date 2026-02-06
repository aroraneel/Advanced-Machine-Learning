# Customer Churn Prediction using AdaBoost Classifier

## 📌 Overview
This project predicts whether a telecom customer will **churn (leave the service)** using the **AdaBoost boosting algorithm**.

Customer churn prediction is a critical business problem in the telecom industry, helping companies improve retention strategies and reduce revenue loss.

The model is trained on the **Telco Customer Churn Dataset** and evaluated using classification metrics.

---

## 🎯 Objectives
- Load and explore telecom customer churn data  
- Encode categorical customer attributes into numeric format  
- Train an **AdaBoost Classifier** with decision tree stumps  
- Evaluate churn prediction performance using:
  - Accuracy Score  
  - Confusion Matrix  
  - Classification Report  

---

## 📁 Dataset Information
- Dataset: **Telco Customer Churn Dataset**
- Records: ~7,000 customers  
- Features include:
  - Customer demographics  
  - Subscription services  
  - Payment methods  
  - Contract details  
- Target Variable:
  - `Churn`
  - Yes = Customer leaves  
  - No = Customer stays  

---

## 🔍 Methodology

### 1. Data Loading & Exploration
- Load dataset using Pandas  
- Inspect dataset shape, columns, statistics  
- Check for missing values and unique categorical values  

---

### 2. Data Preprocessing
- Apply **Label Encoding** to convert categorical columns into numeric values  
- Store encoding mappings for transparency  

---

### 3. Feature & Target Split
- Features (`X`) → All columns except `Churn`  
- Target (`y`) → Customer churn label  

---

### 4. Train-Test Split
- Training Set: 80%  
- Testing Set: 20%  
- Random State fixed for reproducibility  

---

### 5. Model Training (AdaBoost)
Algorithm used:
- **AdaBoost Classifier**
- Weak learner: Decision Tree (max_depth = 1)
- Boosting parameters:
  - n_estimators = 300  
  - learning_rate = 0.5  

AdaBoost improves performance by combining multiple weak learners into a strong classifier.

---

### 6. Model Evaluation
Performance is measured using:
- **Accuracy Score**
- **Confusion Matrix Heatmap**
- **Precision, Recall, F1-score Report**

---

## 📊 Results & Insights
- AdaBoost effectively identifies churn-prone customers  
- Boosting improves prediction accuracy over single decision trees  
- Confusion matrix highlights churn vs non-churn classification behavior  

---

## 🛠️ Tools & Libraries
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 🚀 Applications
- Telecom customer retention strategies  
- Subscription cancellation prediction  
- Marketing targeting for high-risk customers  
- Business decision support systems  

---

## 👤 Author
**Neel Arora**  
BCA Undergraduate | Data Science & Machine Learning Enthusiast  

---
