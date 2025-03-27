# CreditCardFraudPred
# Overview
This project develops a fraud detection model for credit card transactions using machine learning. The model identifies fraudulent transactions while minimizing false positives using Random Forest and class imbalance handling techniques.

# Dataset
The dataset (creditcard.csv) from kaggle contains:
Transaction details such as Amount, Time, and Class (0 = Non-Fraud, 1 = Fraud).
High class imbalance (fraud cases are rare).

## Key Features
# Data Preprocessing:
1. Removed unnecessary columns (Time).
2. Removed duplicate records.
3. Normalized the Amount column using StandardScaler.

# Feature Engineering:
1. Transaction_Frequency: Number of times an amount appears in the dataset.
2. Spending_Pattern: Rolling mean of the last five transaction amounts.

# Handling Class Imbalance:
 Used SMOTE (Synthetic Minority Over-sampling Technique) to generate synthetic fraud cases.

# Model Training & Evaluation:
 Used RandomForestClassifier with 50 estimators.

# Evaluated model performance using:
1. Accuracy
2. ROC-AUC Score
3. Precision, Recall, F1-Score
4. Confusion Matrix (Heatmap)
