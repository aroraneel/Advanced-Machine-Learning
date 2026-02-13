# Hotel Booking Special Request Prediction using LightGBM

## 📌 Overview
This project predicts the **number of special requests** made by hotel customers using a **multiclass classification model**.

A **LightGBM (LGBMClassifier)** is trained on the Hotel Bookings dataset to classify customers into different request categories based on booking and demographic features.

The workflow includes data preprocessing, missing value handling, encoding, model training, evaluation, cross-validation, and final conclusion visualization.

---

## 🎯 Objectives
- Predict customer **special request count** (`total_of_special_requests`)
- Perform multiclass classification using LightGBM
- Handle missing values effectively
- Apply one-hot encoding for categorical features
- Evaluate model using:
  - Accuracy Score
  - Weighted F1 Score
  - Classification Report
  - Confusion Matrix
  - Cross Validation Accuracy
- Visualize final actual vs predicted distribution

---

## 📁 Dataset Information
- Dataset: **Hotel Bookings Dataset**
- Target Column:
  - `total_of_special_requests`

### Target Meaning
Each class represents the number of requests made by a guest:

- 0 → No requests  
- 1 → One request  
- 2+ → Multiple requests  

---

## 🔍 Methodology

### 1. Data Cleaning
Several irrelevant or leakage-prone columns are removed:

- Reservation status fields  
- Cancellation column  
- Agent/company IDs  
- Arrival date details  

---

### 2. Missing Value Handling
Missing values are visualized using a bar chart and then filled:

- `children` → Median imputation  
- `country` → Mode imputation  

---

### 3. Data Visualization
A countplot is used to inspect the distribution of the target variable:

- Helps understand class imbalance across request categories

---

### 4. Feature Encoding
Categorical features are converted into numerical format using:

- One-hot encoding (`pd.get_dummies`)

Encoded dataset shape is printed for verification.

---

### 5. Train-Test Split
Dataset is split into:

- 80% Training  
- 20% Testing  

Stratified sampling ensures balanced class distribution.

---

## 🚀 Model Development (LightGBM)

### Algorithm Used
- **LGBMClassifier (Multiclass Objective)**

### Key Hyperparameters
- `n_estimators = 2000`
- `learning_rate = 0.05`
- `num_leaves = 128`
- `subsample = 0.8`
- `colsample_bytree = 0.8`
- `class_weight = balanced`

LightGBM is chosen for its speed and high performance on structured datasets.

---

## 📊 Model Evaluation

### Metrics Reported
- Accuracy Score  
- Weighted F1 Score  
- Detailed Classification Report  

---

### Confusion Matrix
A heatmap confusion matrix is plotted to visualize multiclass prediction performance.

---

### Cross Validation
5-Fold Cross Validation is performed to ensure model stability:

- Individual accuracy scores are printed
- Mean CV accuracy is calculated

---

## 📉 Final Conclusion Plot
A comparison plot is generated:

- Actual vs Predicted class distribution  
- Provides a clear final summary of model behavior

---

## 🛠️ Tools & Libraries
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- LightGBM  

---

## 🚀 Applications
- Hotel guest behavior prediction  
- Customer service personalization  
- Booking demand analysis  
- Hospitality business intelligence  

---

## 👤 Author
**Neel Arora**  
BCA Undergraduate | Data Science & Machine Learning Enthusiast  

---
