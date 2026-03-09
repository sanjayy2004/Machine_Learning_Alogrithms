 Linear Discriminant Analysis (LDA) using the Digits dataset for supervised dimensionality reduction and digit classification, comparing LDA with Logistic Regression to achieve ~71% accuracy.
​Overview
The notebook loads 1797 8x8 pixel digit images (64 features, 10 classes), preprocesses with standardization, applies LDA to reduce to 2 components (n_classes-1=9 max, but uses 2), and evaluates classification performance.
​Key Steps Implemented
Data Loading: load_digits() creates DataFrame with pixel features and targets (balanced: ~174-183 per class 0-9).
​

Train-Test Split: 80/20 split (1437 train, 360 test) with random_state=3.
​

Standardization: StandardScaler ensures zero mean/unit variance across features to prevent scale bias.
​

LDA Application: LinearDiscriminantAnalysis(n_components=2) fits on train, transforms to LD1/LD2; visualizes scatter plot colored by true labels.
​

Classification: LogisticRegression on LDA features; predicts test set.
​

Results
Metric	Value
Train Shape (post-LDA)	(1437, 2) 
​
Test Shape (post-LDA)	(360, 2) 
​
Test Accuracy	0.714 
​
Confusion matrix shows strong performance on classes 0/4 (97-100% recall) but weaker on 7/5 (36-61%).
​
