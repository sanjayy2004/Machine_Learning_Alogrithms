📊 PCA Hands-On Implementation

This repository contains a comprehensive Jupyter Notebook demonstrating Principal Component Analysis (PCA) implemented from scratch, along with comparisons using scikit-learn. The project focuses on dimensionality reduction and classification using the Digits dataset.

🚀 Overview

This notebook walks through PCA step-by-step, covering:

Data loading and preprocessing

Covariance matrix computation

Eigenvalues and eigenvectors calculation

Explained variance analysis

Dimensionality reduction

Classification using Logistic Regression

The goal is to reduce the original 64-dimensional dataset while preserving approximately 95% of the variance, followed by evaluating model performance.

📂 Dataset

Digits Dataset

1797 samples of handwritten digits

Each image: 8×8 grayscale (64 features)

🔑 Key Steps Implemented
1. Data Loading

Uses load_digits() dataset

Visualizes sample digit images

2. Preprocessing

Mean-centering of data

Feature normalization

3. Covariance Matrix

Computes a 64×64 covariance matrix

Captures feature correlations

4. Eigendecomposition

Computes:

Eigenvalues

Eigenvectors

Sorts components by importance

5. Explained Variance

Calculates:

Individual variance ratio

Cumulative variance

Scree plot visualization

~89% variance captured by first 29 components

6. PCA Transformation
🔹 Manual PCA

Projects data onto top 27 components (~95% variance)

🔹 Scikit-learn PCA

Uses PCA(n_components=0.95)

Output shape: (1797, 29)

7. Classification

Train/test split: 75/25

Model: Logistic Regression

Evaluated on PCA-transformed data

📈 Results
Method	Components	Test Accuracy
Sklearn PCA	29	0.96
Manual PCA	27	0.96
📊 Visualizations

The notebook includes:

Digit image samples

Covariance matrix heatmap

Scree plot (variance explained)

Cumulative variance plot

Model performance comparison

🛠️ Technologies Used

Python

NumPy

Pandas

Matplotlib

Scikit-learn

it pull requests!
