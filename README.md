# 📊 Customer Churn Prediction

This project builds and evaluates machine learning models to predict customer churn using telecom data. It includes data preprocessing, model training, performance evaluation, and feature importance analysis.

## 🧠 Overview

Customer churn is a critical metric for telecom companies. This project uses three classification models—Logistic Regression, Decision Tree, and Random Forest—to identify customers likely to leave the service.

## 📁 Dataset

- **Source**: `Customer-Churn.csv`
- **Size**: 7,043 entries, 20 features
- **Target Variable**: `Churn` (binary: 0 = No churn, 1 = Churn)

## 🔧 Preprocessing Steps

- Dropped irrelevant columns (`customerID`)
- Converted `TotalCharges` to numeric and filled missing values with median
- Encoded categorical features using `LabelEncoder`
- Scaled numerical features using `StandardScaler`
- Split data into training and testing sets (80/20)

## 🧪 Models Used

| Model              | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.76     | 0.53      | 0.84   | 0.65     | 0.86    |
| Decision Tree       | 0.73     | 0.48      | 0.46   | 0.47     | 0.64    |
| Random Forest       | 0.81     | 0.69      | 0.47   | 0.56     | 0.84    |

## 📈 Visualizations

- Confusion matrices for each model
- ROC curve comparison
- Feature importance:
  - Logistic Regression (Odds Ratios)
  - Random Forest (Gini Importance)

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Customer-Churn-Model.git
   cd Customer-Churn-Model
