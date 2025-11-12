# Banking-Churn-Prediction
This notebook performs a full end-to-end Banking Customer Churn Analysis using synthetic data.
# 🏦 Banking Customer Churn Prediction (Machine Learning Project)

This project builds an *end-to-end machine learning pipeline* to predict whether a bank customer will *churn* (leave the bank).  
The dataset is *synthetic*, containing realistic demographic and financial features, along with intentionally added duplicates and missing values to simulate real-world data issues.

---

## 📊 Project Workflow

### 1️⃣ Data Generation & Issues
- Created a synthetic dataset with:
  - Customer demographics and account behavior
  - ~5% duplicate rows
  - ~10% missing values across multiple columns

### 2️⃣ Exploratory Data Analysis (EDA)
- Checked for missing values and duplicates  
- Explored summary statistics and feature distributions

### 3️⃣ Data Cleaning & Preprocessing
- Removed duplicates  
- Imputed missing values using pipelines  
- Scaled numeric features and one-hot encoded categorical ones

### 4️⃣ Model Training
Trained and evaluated three models:
- Logistic Regression  
- Random Forest  
- Gradient Boosting  

Each model was integrated into a Scikit-Learn pipeline for consistent preprocessing and evaluation.

### 5️⃣ Evaluation Metrics
| Metric | Description |
|---------|--------------|
| Accuracy | Overall correctness |
| Precision | Correctly predicted churns / all predicted churns |
| Recall | Correctly predicted churns / all actual churns |
| F1-Score | Balance between Precision & Recall |
| ROC-AUC | Model’s ability to distinguish churn vs. non-churn |

### 6️⃣ Visualization
- ROC curves for all models  
- Confusion matrix for the best model  
- Feature importances and top coefficients  
- Predicted churn probabilities for new customers  

### 7️⃣ Future Predictions
Generated churn probabilities for new unseen customers to simulate deployment usage.

---

## 🏆 Best Model
*Logistic Regression* performed best by ROC-AUC in this run.

---

## 📁 Output Files
| File | Description |
|------|--------------|
| bank_churn_with_issues.csv | Original data with duplicates & missing values |
| bank_churn_cleaned.csv | Cleaned dataset |
| model_comparison_results.csv | Model performance metrics |
| Visualizations | ROC, confusion matrix, feature importance plots |
