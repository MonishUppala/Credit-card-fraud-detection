# Credit Card Fraud Detection using XGBoost and SMOTE

## Overview

This project detects fraudulent credit card transactions using Machine Learning techniques.
Due to extreme class imbalance in fraud datasets, SMOTE (Synthetic Minority Oversampling Technique) was used to balance the training data before training an XGBoost classifier.

The project compares baseline Logistic Regression performance with XGBoost + SMOTE and demonstrates significant improvement in fraud recall.

---

## Dataset

Dataset used:

* Kaggle Credit Card Fraud Detection Dataset

Features:

* Transactions are anonymized using PCA transformation
* Includes:

  * Time
  * Amount
  * V1 to V28
  * Class (Target Variable)

Target:

* `0` → Legitimate Transaction
* `1` → Fraudulent Transaction

Note: The dataset is not included in this repository due to GitHub file size limitations.
You can download it from Kaggle and place `creditcard.csv` inside the `data/` directory.


---

## Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Imbalanced-learn (SMOTE)
* Jupyter Notebook

---

## Workflow

1. Data Loading and Exploration
2. Missing Value Analysis
3. Class Imbalance Visualization
4. Baseline Logistic Regression
5. SMOTE Oversampling
6. XGBoost Model Training
7. Performance Evaluation
8. Feature Importance Visualization
9. Model Saving using Joblib

---

## Model Performance

### Logistic Regression

* High overall accuracy
* Lower fraud recall
* More fraud cases missed

### XGBoost + SMOTE

* Significant improvement in fraud detection recall
* Reduced false negatives
* Better performance on imbalanced data

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC Score
* Confusion Matrix

---

## Results

### Baseline Logistic Regression

* False Negatives: 31

### XGBoost + SMOTE

* False Negatives Reduced To: 10

This demonstrates the effectiveness of SMOTE and XGBoost in handling highly imbalanced fraud detection datasets.

---

## Project Structure

credit-card-fraud-detection/

├── data/

├── notebooks/

├── models/

├── outputs/

├── requirements.txt

├── README.md

└── .gitignore

---

## Future Improvements

* Hyperparameter tuning
* Real-time fraud detection API
* Streamlit deployment
* Deep learning models
* Explainable AI using SHAP values

---

## Author

Monish Uppala
