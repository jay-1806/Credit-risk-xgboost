# Credit Risk Prediction System Using XGBoost & Explainable AI

**Author:** Jay (jay-1806)  
**Project Type:** ML Project  
**Tech Stack:** Python, XGBoost, SHAP, Pandas, Scikit-learn, Streamlit

---

## Overview

This project implements a robust credit risk prediction system using XGBoost on open LendingClub loan data. The goal is to accurately classify borrowers by risk level and provide model interpretability suitable for financial audits.

**Highlights:**
- Achieved ROC-AUC of **92%** on the test set.
- Used SHAP for explainable AI and feature importance.
- Automated feature engineering pipeline.
- Interactive Streamlit dashboard for analysis and visualization.

---

## Dataset

- **Source:** [LendingClub Loan Data](https://www.lendingclub.com/info/download-data.action)
- **Features:** Borrower demographics, loan characteristics, payment history, etc.
- **Target:** Loan default (binary classification)

---

## Methodology

1. **Data Preprocessing:**  
   - Cleaning missing values
   - Encoding categorical variables
   - Feature scaling & selection

2. **Feature Engineering:**  
   - Automated using Pandas & Scikit-learn pipelines
   - Creation of domain-relevant features (e.g., debt-to-income ratio, revolving utilization)

3. **Modeling:**  
   - XGBoost classifier with hyperparameter tuning
   - Cross-validation for robust performance estimates

4. **Explainability:**  
   - SHAP values to interpret predictions
   - Individual borrower explanations for audit purposes

5. **Deployment:**  
   - Streamlit app for interactive visualization
   - Dashboard shows risk segments and explanation plots

---

## Results

- **ROC-AUC:** 0.92 (Test Set)
- **Top Features:** Income, loan amount, credit score, revolving utilization
- **Interpretability:** SHAP summary and force plots

---

## Streamlit Dashboard

![](assets/dashboard_screenshot.png) <!-- Add your Streamlit dashboard screenshot here -->

**Features:**
- Upload borrower data and get risk predictions
- Visualize feature contributions (SHAP)
- Segment analysis for risk groups

---

## Getting Started

### Prerequisites

- Python 3.8+
- pip

### Installation

```bash
git clone https://github.com/jay-1806/credit-risk-xgboost
cd credit-risk-xgboost
pip install -r requirements.txt
```

### Usage

#### Train Model

```bash
python train.py --data data/loan_data.csv
```

#### Run Dashboard

```bash
streamlit run app.py
```

---

## File Structure

```
credit-risk-xgboost/
│
├── data/                  # Raw and processed data
├── notebooks/             # Jupyter notebooks for EDA & experiments
├── src/                   # Source code (model, preprocessing, utils)
├── app.py                 # Streamlit dashboard
├── train.py               # Training script
├── requirements.txt
└── README.md
```

---

## Academic Integrity

This project is academically motivated and all code is original. LendingClub data is used for educational purposes only.

---

## License

MIT License

---

## Contact

For academic questions or collaboration:  
**Jay** | [GitHub](https://github.com/jay-1806)
