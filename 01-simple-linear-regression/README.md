# 📈 Linear Regression on Insurance Charges Dataset

End-to-end Linear Regression project predicting insurance charges using a
real-world insurance dataset.

The project covers the complete machine learning workflow including
EDA, feature engineering, model training, evaluation, and visualization.

---


## 📋 Key Steps Covered

### 1️⃣ Data Loading & Exploration
- Loaded dataset using Pandas
- Performed Exploratory Data Analysis (EDA)
- Analyzed feature distributions
- Checked correlations between variables
- Handled missing values

---

### 2️⃣ Feature Engineering
- Checked multicollinearity using Variance Inflation Factor (VIF)
- Identified high VIF features:
  - age ≈ 13.55
  - bmi ≈ 14.52
- Removed highly correlated features to reduce multicollinearity
- Reduced VIF values below threshold (< 10)
- Applied label encoding on categorical features:
  - sex
  - smoker
  - region

---

### 3️⃣ Model Training
- Selected relevant features after preprocessing
- Split data into training and testing sets (80/20)
- Trained Linear Regression model using `sklearn.linear_model.LinearRegression`
- Model trained on features such as:
---

### 4️⃣ Model Evaluation

| Metric | Value |
|------|------|
| Mean Squared Error (MSE) | 2,674,836 |
| Root Mean Squared Error (RMSE) | 1,635.49 |
| R² Score | 85.96% |

---

### 5️⃣ Visualization & Error Analysis
- Regression plots to visualize predictions
- Compared actual vs predicted insurance charges
- Performed error analysis to evaluate model performance

---

## 🛠 Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels (for VIF calculation)
- Jupyter Notebook

---

## 🧠 Key Learnings
- Importance of EDA before model building
- Impact of multicollinearity on regression models
- Using VIF to select stable features
- Encoding categorical variables correctly
- Evaluating regression models using multiple metrics


---

## 📌 Conclusion
This project demonstrates a complete and practical implementation of
Linear Regression, focusing on data understanding, feature engineering,
and model evaluation using a real-world insurance dataset.

---


