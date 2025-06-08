# 💼 LoanTap Logistic Regression Project

---

## 🏢 About LoanTap

**LoanTap** is an online fintech platform focused on delivering **customized personal loan solutions** to millennials and salaried professionals. Their mission is to simplify the credit experience by offering **instant, flexible, and borrower-friendly loans**. LoanTap provides four major types of financial products:
- Personal Loan
- EMI-Free Loan
- Personal Overdraft
- Advance Salary Loan

This project specifically focuses on the **Personal Loan** underwriting process, where the goal is to determine a borrower's **creditworthiness** using predictive analytics and machine learning.

---

## 📁 Project Files

- `LoanTap Logistic Regression.ipynb`: The complete notebook including data exploration, preprocessing, logistic regression modeling, evaluation, and insights.
- `read_me.md`: A brief overview of the business problem, dataset, methodology, and results.

---

## 🎯 Objective

To build a **Logistic Regression Classification Model** that predicts whether a borrower will **fully repay** or **default (charged-off)** on a **personal loan**. The aim is to support LoanTap’s **underwriting system** in making smarter, data-driven loan approval decisions.

---

## 🧾 Feature Details

The dataset includes **396,030 entries** and **27 variables**, categorized as follows:

### 🔹 Loan & Credit Details
- `loan_amnt`: Requested loan amount
- `term`: Duration of the loan (36/60 months)
- `int_rate`: Interest rate
- `installment`: Monthly payment amount
- `grade`, `sub_grade`: LoanTap-assigned risk grades
- `dti`: Debt-to-income ratio
- `revol_bal`: Total revolving balance
- `revol_util`: Revolving utilization rate
- `total_acc`: Total credit lines
- `open_acc`: Open credit lines
- `pub_rec`: Public derogatory records
- `pub_rec_bankruptcies`: Number of bankruptcies

### 🔹 Employment & Income Information
- `emp_title`: Job title
- `emp_length`: Years of employment
- `annual_inc`: Annual income

### 🔹 Ownership & Application Info
- `home_ownership`: Rent, Mortgage, Own, etc.
- `application_type`: Individual or joint application
- `verification_status`: Income verification status

### 🔹 Timeline & Credit History
- `issue_d`: Loan issuance month
- `earliest_cr_line`: First credit line date
- `mort_acc`: Mortgage accounts

### 🔹 Target & Identifiers
- `loan_status`: **Target Variable** (Fully Paid or Charged Off)
- `purpose`: Loan purpose category
- `title`: Loan title entered by borrower
- `initial_list_status`: Public listing status
- `address`: Borrower's address

---

## 🛠 Tools & Libraries Used

- **Python Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `warnings`
- **Machine Learning**: `scikit-learn`, `LogisticRegression`, `StandardScaler`, `train_test_split`
- **Encoding**: `category_encoders` for Target Encoding
- **Evaluation**: Accuracy, Precision, Recall, F1-score, ROC-AUC, Confusion Matrix

---

## 🌟 Key Highlights

- ✅ Performed **extensive EDA** using countplots, boxplots, histograms, and heatmaps
- ✅ Cleaned and preprocessed data with **missing value imputation**, **feature encoding**, and **column transformations**
- ✅ Built and validated a **Logistic Regression model** with:
  - **Validation Accuracy**: ~80.4%
  - **Precision**: ~81.2%
  - **Recall (Sensitivity)**: ~98.4%
  - **F1-Score**: ~88.9%
  - **ROC-AUC Score**: 0.70
- ✅ High recall with low false negatives, but relatively higher false positives suggest **bias towards positive prediction**

---

## ✅ Conclusion

This project demonstrates a complete machine learning pipeline for **credit risk modeling**. The **Logistic Regression** model is a solid baseline with high recall, helping effectively flag potential **safe borrowers**. However, further improvements can be made by:
- Trying **ensemble models** (Random Forest, XGBoost)
- **Cost-sensitive learning** for class imbalance
- Fine-tuning thresholds for better **precision-recall balance**

This approach helps LoanTap make **informed lending decisions**, reduce default risk, and serve customers with **responsible credit products**.

---
