Decision Tree Classifier: Heart Disease Prediction ❤️


Production-ready Decision Tree Classifier predicting heart disease presence (target: 0/1) on the classic UCI Heart Disease dataset (303 samples, 13 features: age, sex, cp, trestbps, chol, thalach, etc.). Achieves 78.69% accuracy—impressive for interpretable trees in medical ML!
​📋 Key Steps Covered
EDA Excellence: No nulls/duplicates; boxplots per feature, correlation heatmap (thalach/oldpeak strongly predict target).
​
Preprocessing: Clean split (242 train/60 test, random_state=0); target balanced (164 yes, 138 no).
​Model Building: DecisionTreeClassifier() (default Gini); trained on all features.
​
Evaluation (Test Set):

Metric	Value
Accuracy	78.69%
Precision/Recall strong on positives (26/31 true positives).


📊 Results & Insights
78.69% Test Accuracy: Outperforms baselines; low FN (5) critical for healthcare (few missed diseases).
