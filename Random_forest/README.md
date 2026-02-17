Random Forest Classifier: Wine Fraud Detection 🍷🔍
[
[
[
[
dataset link : https://drive.google.com/file/d/1q89o1bEVy4mLcr464hC_4-r30V5JQIOz/view?usp=sharing

Production-grade Random Forest detecting wine fraud (quality: Legit/Fraud) on UCI Wine dataset (6497 samples → 3812 after dedup, 12 features: fixed acidity, volatile acidity, density, etc.). 98.1% accuracy post-SMOTE balancing (743 Legit, 20 Fraud test)—ensemble power crushes baselines!
​

📋 Key Steps Covered
EDA Mastery: No nulls; 1177 dups dropped; severe imbalance (6251 Legit vs 246 Fraud); boxplots per feature.
​

Preprocessing: LabelEncoder (type/quality); SMOTE oversamples minority to 3687:3687; 80/20 split (3049 train).
​

Model: RandomForestClassifier() (default 100 trees); tuned n_estimators= (~97.3-97.4%).
​

Evaluation (Test: 763 samples):

Metric	Value
Accuracy	98.1%
Predictions	762 Legit, 1 Fraud
Actual Test	743 Legit, 20 Fraud

📊 Results & Insights
98.1% Test Accuracy: Near-perfect; SMOTE fixes imbalance—critical for fraud detection (low FN)
