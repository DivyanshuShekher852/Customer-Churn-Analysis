
# 📊 Customer Churn Analysis

## 📌 Project Overview

Customer churn is an important business problem because customer cancellations directly affect recurring revenue and long-term customer value.

This project analyzes a **15-customer subscription dataset** to identify churn patterns, calculate retention metrics, estimate Customer Lifetime Value (CLV), measure Monthly Recurring Revenue (MRR) at risk, and identify key behavioral drivers of churn.

> **Note:** This is a small illustrative dataset. Results should be treated as directional insights and validated using a larger production dataset.

---

## 🎯 Objectives

The main objectives of this project are to:

* Calculate the **Churn Rate**
* Calculate the **Retention Rate**
* Estimate **Customer Lifetime Value (CLV)**
* Calculate **Monthly Recurring Revenue (MRR) Loss**
* Analyze churn by **Contract Type**
* Analyze churn by **Payment Method**
* Analyze churn by **Subscription Tier**
* Analyze churn by **Customer Tenure**
* Investigate **Support Ticket Volume**
* Identify high-risk customer segments
* Provide actionable business recommendations

---

## 🛠️ Technologies Used

| Technology       | Purpose                    |
| ---------------- | -------------------------- |
| Python           | Data analysis              |
| Pandas           | Data cleaning and analysis |
| NumPy            | Numerical calculations     |
| Matplotlib       | Data visualization         |
| Seaborn          | Statistical visualizations |
| Jupyter Notebook | Development environment    |

---

## 📂 Project Workflow

```text
Customer Churn Analysis
│
├── Data Loading
├── Data Inspection
├── Data Cleaning
├── Exploratory Data Analysis
├── Churn Rate Calculation
├── Retention Rate Calculation
├── CLV Analysis
├── MRR Loss Analysis
├── Contract Analysis
├── Payment Method Analysis
├── Tenure Analysis
├── Support Ticket Analysis
├── Data Visualization
├── Key Findings
└── Business Recommendations
```

---

## 📈 Key Metrics

The dataset contains **15 customers**, with **8 retained customers and 7 churned customers**, resulting in a **46.7% churn rate**.

| Metric                 |        Result |
| ---------------------- | ------------: |
| Total Customers        |            15 |
| Retained Customers     |             8 |
| Churned Customers      |             7 |
| Churn Rate             |         46.7% |
| Total MRR              |     $1,269.85 |
| MRR Lost to Churn      | $409.93/month |
| MRR at Risk            |         32.3% |
| Average Monthly Charge |        $84.66 |
| Average CLV            |     $1,591.55 |

---

## 🔍 Key Findings

### 1. Contract Type

Contract type was the strongest churn signal in the sample.

* **Month-to-Month:** 100% churn
* **One-Year:** 0% churn
* **Two-Year:** 0% churn

Every month-to-month customer churned, while all customers with longer contracts were retained.

### 2. Customer Tenure

Churn was heavily concentrated among newer customers.

* **0–6 months:** 100% churn
* **13–24 months:** 20% churn
* **25+ months:** 0% churn

This indicates that the first year is the most important retention period.

### 3. Support Tickets

Churned customers generated significantly more support tickets.

* Churned customers: **4.3 tickets on average**
* Retained customers: **1.0 ticket on average**

This suggests that support friction may be an important early-warning signal for churn.

### 4. Subscription Tier

The Basic tier showed the highest observed churn.

* **Basic:** 71.4%
* **Pro:** 50%
* **Enterprise:** 0%

The results suggest that the value proposition and engagement of Basic-tier customers should be investigated.

### 5. Payment Method

Observed churn varied significantly by payment method.

* **Debit Card:** 100%
* **UPI:** 75%
* **Credit Card:** 33.3%
* **Bank Transfer:** 0%

Payment friction may therefore be worth investigating, although the small sample prevents strong causal conclusions.

---

## 💡 Business Recommendations

### 1. Encourage Contract Upgrades

Encourage month-to-month customers to move to annual or longer contracts through discounts, bonuses, or additional features.

### 2. Strengthen the First 90 Days

Introduce proactive onboarding and customer-success check-ins during the first three months.

### 3. Reduce Support Friction

Prioritize faster resolution of common issues affecting new customers and monitor customers with unusually high ticket volumes.

### 4. Review the Basic Tier

Evaluate the Basic plan's features, pricing, and upgrade path to improve customer stickiness.

### 5. Audit Payment Processes

Investigate high-churn payment methods and consider payment retries, failure alerts, and easier payment options.

### 6. Build a Churn-Risk Indicator

Create a simple customer-risk score using **tenure and support-ticket volume** to help customer-success teams prioritize intervention.

---

## 📊 Visualizations

The project includes:

* Churn distribution chart
* Churn rate by contract type
* Churn rate by payment method
* Churn rate by subscription tier
* Churn rate by tenure
* Support tickets vs. churn boxplot
* Tenure vs. churn boxplot
* Contract Type × Payment Method heatmap
* Correlation heatmap

---

## 📁 Project Deliverables

```text
Customer-Churn-Analysis/
│
├── customer_churn_sample.csv
├── customer_churn_analysis.ipynb
├── customer_churn_cleaned.csv
├── customer_churn_summary.csv
├── churn_by_contract.csv
├── churn_by_payment_method.csv
├── churn_by_tenure.csv
├── Customer_Churn_Analytics_Report.pdf
└── README.md
```

---

## ⚠️ Limitations

The dataset contains only **15 records**, making it unsuitable for statistically robust conclusions. The results are useful for demonstrating the analytical workflow but should be validated against a much larger customer dataset before implementing business-wide retention strategies.

---

## 🏁 Conclusion

The analysis indicates that churn in this sample is **front-loaded and strongly associated with month-to-month contracts, short customer tenure, and higher support-ticket volume**.

The most immediate retention opportunity is to **move new customers away from month-to-month billing, improve the first 90 days of onboarding, and resolve support issues quickly**.

---

## 👨‍💻 Project Type

**Data Analytics | Customer Retention | Exploratory Data Analysis | Business Intelligence**

**Author:** Divyanshu Shekher
