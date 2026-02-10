# 📊 Telco Customer Churn – Exploratory Data Analysis (EDA)

## 🔍 Project Overview

Customer churn is a major challenge for subscription-based businesses. This project focuses on performing **Exploratory Data Analysis (EDA)** on the **Telco Customer Churn dataset** to understand customer behavior, identify churn patterns, and prepare the data for machine learning models.

The dataset is sourced from **Kaggle** and contains demographic information, service usage details, billing information, and churn-related attributes of telecom customers.

---

## 📁 Dataset Information

* **Source:** Kaggle – Telco Customer Churn Dataset
* **Total Records:** 7,043 customers
* **Total Features:** 26 (after encoding)
* **Target Variable:** `Churn Label` / `Churn Value`

### 🔑 Feature Categories

* **Demographic:** Gender, Senior Citizen, Partner, Dependents
* **Account Information:** Tenure Months, Contract, Payment Method, Paperless Billing
* **Services:** Phone Service, Internet Service, Online Security, Streaming TV, etc.
* **Financial:** Monthly Charges, Total Charges, CLTV
* **Churn Details:** Churn Label, Churn Score, Churn Reason

---

## 🛠️ Tools & Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## 🧪 EDA Workflow

### 1️⃣ Data Loading & Initial Inspection

* Loaded dataset using Pandas
* Checked shape, column names, and sample records
* Used `df.info()` and `df.describe()` for structure and summary

### 2️⃣ Data Cleaning

* Verified **no missing values** across all columns
* Corrected data types (e.g., converting numeric columns from object to float)
* Ensured logical consistency of categorical variables

### 3️⃣ Categorical Variable Handling

Categorical features were divided into:

#### 🔹 Binary Categorical (Label Encoding)

Examples:

* Phone Service
* Multiple Lines
* Online Security
* Streaming TV
* Contract

✔ Converted to numeric values using Label Encoding

#### 🔹 Nominal Categorical (One-Hot Encoding)

Examples:

* Internet Service
* Payment Method

✔ Applied One-Hot Encoding to avoid ordinal bias

---

### 4️⃣ Feature Engineering

* Encoded all categorical variables
* Converted boolean columns to numerical format if required
* Ensured dataset contains **only numerical values** for modeling

---

### 5️⃣ Final Dataset Validation

* Rechecked dataset using `df.info()`
* Confirmed:

  * No missing values
  * No object-type columns
  * Suitable for ML algorithms

✔ Dataset is **cleaned_telco_churn**

---

## 📈 Key Insights from EDA

* Customers with **month-to-month contracts** show higher churn
* **Higher monthly charges** are associated with increased churn
* Customers without **online security or tech support** churn more
* **Fiber optic internet users** show higher churn compared to DSL

---

## 🚀 Conclusion

This EDA process transformed raw telecom customer data into a clean, structured, and machine-learning-ready dataset. The insights gained can help businesses design better retention strategies and serve as a strong foundation for predictive churn modeling.

---

## 📎 Author

**Anakha Jose**
Data Science | Machine Learning | Python

---
