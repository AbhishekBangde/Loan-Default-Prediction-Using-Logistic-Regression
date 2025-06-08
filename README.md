# 📊 LoanTap Logistic Regression

## 📁 Project Files

- **LoanTap Logistic Regression.ipynb**: Contains data exploration, preprocessing, model building, evaluation, and insights.
- **read_me.md**: Provides business context, data understanding, and project overview.

---

## 🎯 ## Objective

To build a **logistic regression classification model** that predicts whether a borrower will **fully repay** or **default (charged-off)** on a personal loan issued through LoanTap. The model assists in automating and enhancing the **underwriting process** based on borrower financial and demographic data.

---

## 🧾 ## Feature Details

The dataset contains **396,030 rows** and the following **27 features**:

### 📌 Loan & Credit Attributes:
- `loan_amnt`: Loan amount requested
- `term`: Loan duration (36 or 60 months)
- `int_rate`: Interest rate
- `installment`: Monthly installment amount
- `grade`: LoanTap-assigned grade
- `sub_grade`: Sub-categorization of loan grade
- `dti`: Debt-to-income ratio
- `revol_bal`: Total revolving balance
- `revol_util`: Revolving credit utilization
- `total_acc`: Total number of credit lines
- `open_acc`: Number of open credit lines
- `pub_rec`: Public derogatory records
- `pub_rec_bankruptcies`: Number of bankruptcies

### 📌 Employment & Income:
- `emp_title`: Job title
- `emp_length`: Employment duration (in years)
- `annual_inc`: Annual income

### 📌 Ownership & Application:
- `home_ownership`: Home ownership status (RENT, MORTGAGE, OWN)
- `application_type`: Individual or joint loan application
- `verification_status`: Income verification status

### 📌 Timeline & History:
- `issue_d`: Date of loan issuance
- `earliest_cr_line`: Date of earliest credit line
- `mort_acc`: Number of mortgage accounts

### 📌 Target & Identifiers:
- `loan_status`: **Target Variable** – Fully Paid or Charged Off
- `purpose`: Reason for taking the loan
- `title`: Loan title from borrower
- `initial_list_status`: Loan listing type (W or F)
- `address`: Customer address

---

## 🛠 ## Tools & Libraries Used

- **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `warnings`
- **Machine Learning**: `scikit-learn`, `category_encoders`
- **Techniques**: Target Encoding, Standard Scaling, Logistic Regression
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score, Confusion Matrix, ROC-AUC

---

## 🌟 ## Key Highlights

- 🔍 **Exploratory Data Analysis**: Countplots, boxplots, heatmaps, histograms to visualize feature relationships with loan status.
- 🧹 **Data Cleaning**: Missing values imputed using mode and mean; irrelevant columns dropped; categorical encoding performed.
- 📉 **Model Training**: Logistic Regression built using encoded and scaled features.
- 🧪 **Performance**:
  - **Accuracy**: ~80.4% (validation)
  - **Precision**: ~81.2%
  - **Recall (Sensitivity)**: ~98.4%
  - **F1-score**: ~88.9%
  - **AUC Score**: 0.70
- ⚠️ **Confusion Matrix** reveals good recall but high false positives (predicting "fully paid" when actually "charged off").

---

## ✅ ## Conclusion

This project demonstrates the complete pipeline of building a **logistic regression model** for **loan default prediction**. While the model performs strongly in identifying safe borrowers, enhancements like **ensemble models** and **cost-sensitive learning** could further improve its ability to capture defaults. Overall, this serves as a robust foundation for **credit risk analytics** in digital lending platforms.

---

