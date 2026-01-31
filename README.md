# 📊 Telco Customer Churn Retention Modelling & KPI Dashboard

## 📌 Project Overview
Customer churn is a major revenue risk for subscription-based businesses.  
This project analyzes telecom customer data to **identify churn patterns**, **build predictive churn models**, and **derive actionable retention strategies**.

The workflow follows an **end-to-end analytics pipeline**:
- **SQL** → Data cleaning & transformation  
- **Power BI** → Executive KPI & churn dashboard  
- **Python** → Churn & retention modeling  

---

## 🎯 Business Objective
- Identify **customers likely to churn**
- Understand **key drivers of churn**
- Enable **targeted retention actions** instead of blanket offers

---

## 🗂 Dataset
- **Rows:** 6,418 customers  
- **Domain:** Telecom subscription data  
- **Key attributes:**
  - Demographics (Age, Gender, State)
  - Account & tenure information
  - Pricing & revenue metrics
  - Contract & service features
  - Customer status (Stayed / Churned)

---

## 🧹 Data Preparation (SQL)
- Standardized categorical values
- Converted blank values to meaningful defaults
- Built a **production-ready table (`prod_Churn`)**
- Preserved raw and semi-cleaned layers for traceability

**Key principle:**  
> Data cleaning handled in SQL, analytics & modeling handled downstream.

---

## 📈 Power BI – Executive KPI Dashboard
Built a **1-page executive dashboard** focused on:
- **Churn Rate**
- **Total Revenue**
- **ARPU**
- **Customer Distribution**

### Key Visuals
- Churn % by Contract Type  
- Churn % and Customer Volume by Age Group  
- Churn by Payment Method & Internet Type  
- Revenue contribution by customer segments  

👉 Designed for **leadership-level decision making**.

---

## 🤖 Python – Churn & Retention Modeling

### Models Used
1. **Logistic Regression** (Baseline, explainable)
2. **Random Forest** (Non-linear benchmark)

### Modeling Steps
- One-hot encoding of categorical variables
- Train-test split with stratification
- Feature scaling for Logistic Regression
- Model comparison using **ROC-AUC**

---

## 📊 Model Evaluation
- ROC Curve
- Precision–Recall Curve
- Confusion Matrix
- Threshold tuning

### Threshold Strategy
Instead of the default 0.5 cutoff, the decision threshold was tuned to:
- **Improve recall for churned customers**
- Prioritize early identification of at-risk users

This aligns with **real-world retention objectives**, where missing churners is more costly than false alarms.

---

## 🔍 Key Insights (Retention Drivers)
- Customers on **month-to-month contracts** churn more
- **Short tenure** is a strong churn signal
- **Higher monthly charges** increase churn risk
- Contract length and pricing are stronger drivers than demographics

---

## 🎯 Retention Strategy (Business Interpretation)
The churn predictions can be used to:
- **Target high-risk customers** (who)
- **Intervene early**, especially during initial tenure (when)
- **Customize retention offers** based on churn drivers (how)

**Examples:**
- Price-sensitive users → discounts or plan optimization  
- Month-to-month users → contract upgrades  
- Early-tenure users → onboarding & engagement programs  

---

## 🧠 Conclusion
This project demonstrates how churn prediction models directly support **retention decision-making**.  
By combining explainable models, non-linear benchmarks, and business-focused evaluation, the solution moves beyond accuracy to **actionable insights**.

---

## 🛠 Tools & Technologies
- **SQL** – Data cleaning & transformation  
- **Power BI** – Executive KPI & churn dashboard  
- **Python** – Pandas, Scikit-learn, Matplotlib  

---

## 📌 Project Type
- ✔ Churn Modeling  
- ✔ Retention Modeling  
- ✔ Product / Customer Analytics  
- ✔ Executive KPI Reporting  

---

## 📬 Author
**Bodhisatva Mukherj**

