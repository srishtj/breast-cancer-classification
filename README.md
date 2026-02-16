# Breast Cancer Classification — Model Benchmarking & Evaluation

## Problem Statement
Early detection of malignant breast tumors is critical in reducing mortality rates.  
This project builds and evaluates multiple machine learning models to classify tumors as malignant or benign using diagnostic imaging features.  

Special emphasis is placed on minimizing false negatives (i.e., misclassifying malignant tumors as benign).

## Methodology

### Data Preparation
- Stratified train-test split (80/20)
- Feature scaling using `StandardScaler` inside a Pipeline to prevent data leakage

### Model Development
Benchmarked models:
1. K-Nearest Neighbors (with hyperparameter tuning)
2. Logistic Regression
3. Random Forest

### Hyperparameter Tuning
Used GridSearchCV with 5-fold cross-validation optimizing macro recall to balance performance across both classes and reduce malignant false negatives.