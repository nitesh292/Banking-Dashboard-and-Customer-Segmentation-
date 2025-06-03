# 💼 Banking Customer Segmentation and Risk Analysis

## 🎯 Project Objective

To analyze a banking dataset and segment customers based on their financial behavior—such as deposits, loans, and credit card balance—to derive actionable insights that can help the bank improve customer targeting, reduce credit risk, and personalize services.

---

## 🛠️ Tools & Technologies Used

- **Python (Jupyter Notebook)**: For Exploratory Data Analysis (EDA) and K-Means clustering  
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn  
- **Power BI**: For building a dynamic and interactive dashboard

---

## 🧾 Project Steps

### 📂 Data Preparation

- Loaded the dataset in Jupyter Notebook
- Conducted data profiling and transformations:
  - Parsed date columns and handled missing values
  - Created meaningful features:
    - `Tenure (Years)`: Duration since customer joined the bank
    - `Loan-to-Deposit Ratio (LDR)`: Indicates customer’s loan burden
    - `Debt-to-Income Ratio (DTI)`: Reflects financial stress level
  - Categorized customers by `Age Group`

---

### 📊 Exploratory Data Analysis (EDA)

> [🔗 View EDA Notebook](Banking%20EDA.ipynb)

- Performed univariate and bivariate analysis:
  - Analyzed distributions of `Estimated Income`, `Credit Card Balance`, `Bank Deposits`, etc.
  - Identified outliers and key variable correlations

---

### 🧠 Customer Segmentation (Clustering)

> [🔗 View Clustering Notebook]

- Selected features for clustering:
  - `Estimated Income`, `Bank Deposits`, `Bank Loans`, `Credit Card Balance`
  - `Superannuation Savings`, `LDR`, `DTI`, `Risk Weighting`
- Applied preprocessing using `StandardScaler`
- Used the **Elbow Method** to determine optimal clusters (K = 4)
- Final customer segments:
  - **High Value**: High income, high deposits, low DTI/LDR
  - **Mid Value**: Average metrics, balanced profile
  - **Low Value**: Low income or low deposits
  - **At Risk**: High debt, low income, high DTI/LDR

---

## 📈 Power BI Dashboard

> [📊 View Dashboard File](Banking%20dashboard.pbix)

### 📌 Dashboard Pages Overview

1. **Overview**  
   Summarizes key metrics: Total Loan, Deposits, LDR, and DTI for holistic performance view

2. **Customer Segmentation**  
   Displays number of customers per segment with corresponding loan, LDR, and DTI distributions

3. **High Risk Customers**  
   Highlights clients with high DTI and LDR, along with risk weighting to prioritize monitoring

4. **Loan and Deposit Analysis**  
   Breaks down:
   - **Loan Components**: Credit Card Balance, Bank Loans, Business Lending  
   - **Deposit Components**: Superannuation, Savings, Checking, Bank Deposits

---

## 📌 Key Insights

- **High Value** customers represent the most profitable segment with stable financial indicators
- **At Risk** customers show elevated loan-to-deposit and debt-to-income ratios—potential credit risk
- **Product penetration** (e.g., credit cards, checking/savings) varies significantly by segment, indicating upsell opportunities
- **Loyalty Classification** and **Occupation** help tailor retention strategies

---

## ✅ Recommendations

- Focus marketing and personalized offerings toward **High Value** and **Mid Value** customers
- Closely monitor **At Risk** customers and establish early warning systems based on DTI and LDR
- Improve cross-sell strategies by analyzing gaps in product ownership across segments

---
