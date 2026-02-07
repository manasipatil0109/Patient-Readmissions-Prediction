# Patient Readmissions Prediction

## Overview
This project presents a machine learning–based hospital readmission prediction system designed to identify diabetic patients at high risk of being readmitted within 30 days. The system helps healthcare providers take timely, preventive actions to improve patient outcomes and reduce operational and financial burdens.

---

## Problem Statement
Hospitals face significant challenges due to high 30-day readmission rates among diabetic patients. Early identification of high-risk patients is critical but difficult due to the scale, complexity, and variability of clinical data. Traditional rule-based approaches lack accuracy and adaptability, necessitating a data-driven predictive solution.

---

## Solution
A supervised machine learning pipeline was developed to predict 30-day hospital readmissions using the UCI Diabetic dataset. The solution includes:

- Multiple classification models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
- Feature selection using Random Forest importance scores and correlation analysis
- Robust data preprocessing:
  - Missing value imputation
  - Label encoding and one-hot encoding
  - Target variable transformation
- Model tuning and evaluation using cross-validation and ROC-AUC optimization

---

## Key Contributions
- Designed an end-to-end machine learning pipeline processing **100K+ patient records** with **50+ clinical features**
- Tuned models using **GridSearchCV**, achieving:
  - **82% ROC-AUC**
  - **75% recall** for high-risk patient detection
- Addressed class imbalance using:
  - Stratified sampling
  - Class weight adjustments
- Visualized model performance using:
  - Confusion matrices
  - ROC curves
  - Classification reports
- Identified key clinical drivers of readmission, including:
  - Number of medications
  - Discharge disposition
  - Time spent in hospital

---

## Engineering Practices
- Followed a **modular and scalable architecture** to ensure reproducibility and future extensibility
- Implemented best practices for:
  - Train-test splitting
  - Cross-validation
  - Hyperparameter tuning
- Maintained clean version control using GitHub
- Tracked experiments to ensure reproducibility and consistent evaluation

---

## Technologies Used
### Languages & Libraries
- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Matplotlib

### Machine Learning Concepts
- Supervised Learning
- Binary Classification
- Feature Engineering
- Imbalanced Dataset Handling
- ROC-AUC Optimization

---

## Impact
This system enables healthcare professionals to proactively manage high-risk diabetic patients, with the potential to reduce 30-day readmission rates by up to **15%**. The insights generated from the model support early intervention strategies and contribute to improved clinical decision-making and patient care.

---

## Dataset
- **UCI Diabetic Readmission Dataset**
- Publicly available and widely used for healthcare analytics research

---

## Future Enhancements
- Integration with real-time hospital EHR systems
- Explainability using SHAP or LIME for clinician trust
- Deployment as a REST API for clinical decision support
- Extension to multi-disease readmission prediction
