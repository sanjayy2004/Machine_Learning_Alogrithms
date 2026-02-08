# 🏦 Logistic Regression – Bank Term Deposit Prediction

Binary classification project using **Logistic Regression** to predict whether a client will subscribe 
to a **bank term deposit** (`y`: yes / no) using the **Bank Marketing dataset**.

This project demonstrates an end-to-end machine learning workflow including data exploration,
preprocessing, feature selection, model training, evaluation, and visualization.

---

## 📂 Dataset Information
- Dataset: Bank Marketing Dataset
- Rows: ~41,000
- Features: 21
 
---

## 📋 Key Steps Covered

### 1️⃣ Data Loading & Exploratory Data Analysis (EDA)
- Loaded dataset from CSV file
- Identified and handled ~4–5 missing values per categorical column
- Removed duplicate records (13 rows)
- Generated statistical summaries using `df.describe()`
- Performed basic exploratory analysis

---

### 2️⃣ Data Preprocessing
- Applied **Label Encoding** on categorical features such as:
  

---

### 3️⃣ Feature Selection
- Used **Recursive Feature Elimination (RFE)** with Logistic Regression
- Selected **top 10 most important features**:
 
### 4️⃣ Model Training
- Split dataset into training and testing sets (80/20)
  - Training samples: ~28,000
  - Testing samples: ~7,000
- Trained model using:
  ```python
  
  LogisticRegression(max_iter=1000)

---
###  Evaluation: 
Metric Value Accuracy 93.43% 
Confusion Matrix [] 
Heatmap visualization of confusion matrix included.​
