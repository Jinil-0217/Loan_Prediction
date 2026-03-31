# Loan Approval Prediction

## 📌 Overview
This project aims to predict whether a loan application will be approved or rejected using machine learning techniques.

## 📊 Dataset
The dataset contains information about applicants such as income, loan amount, credit history, and demographic details.

- Rows: 614
- Columns: 13
- Target Variable: Loan_Status (Approved / Rejected)

---

## 🧹 Data Preprocessing
- Handled missing values using mode (categorical) and median (numerical)
- Converted categorical variables into numerical format
- Removed irrelevant columns (e.g., Loan_ID)

---

## ⚙️ Feature Engineering
Created meaningful financial features:
- Total Income
- Loan-to-Income Ratio
- EMI (LoanAmount / Term)
- Income per Person

These features improved the model's ability to capture financial risk.

---

## 🤖 Models Used
- Logistic Regression (Baseline)
- Logistic Regression with Class Balancing
- Random Forest (Final Model)

---

## ⚖️ Handling Imbalance
- Used `class_weight='balanced'`
- Evaluated models using precision, recall, and F1-score instead of accuracy alone

---

## 📈 Results

| Model | Recall (Reject) | Accuracy |
|------|----------------|----------|
| Logistic Regression | 0.58 | 0.86 |
| Random Forest | 0.63 | 0.82 |

---

## 🔍 Key Insights
- Models were biased toward loan approvals due to class imbalance
- Feature engineering improved detection of risky applicants
- Performance is limited by dataset feature quality

---

## 🧠 Conclusion
Feature engineering had a greater impact on performance than model complexity. The project highlights the importance of domain knowledge in building effective machine learning solutions.

---

## 📦 Requirements
See `requirements.txt`

---

## 🚀 How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt