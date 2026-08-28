# Customer  Shopping Behavior Analysis

An end-to-end data analytics project exploring customer purchasing patterns, demographics, and product preferences. This project leverages **Python** for data cleaning, preprocessing, and exploratory data analysis (EDA), **SQL** for business querying, **Power BI** for interactive dashboards, and an **Executive Presentation** summarizing strategic recommendations.

---

## 📌 Project Overview
The objective is to analyze transaction records and customer demographic data to uncover key revenue drivers, evaluate subscription behaviors, assess discount/promo-code effectiveness, and identify high-value customer segments across regions and product categories.

---

## 📊 Dataset Overview
The dataset contains **3,900 customer records** across **18 raw attributes**, capturing customer demographics, transactions, and behavioral patterns:

* **Customer Demographics:** `Customer ID`, `Age`, `Gender`, `Location`
* **Purchase Details:** `Item Purchased`, `Category`, `Purchase Amount (USD)`, `Size`, `Color`, `Season`
* **Loyalty & Behavioral Metrics:** `Subscription Status`, `Previous Purchases`, `Frequency of Purchases`, `Review Rating`
* **Transaction Attributes:** `Payment Method`, `Shipping Type`, `Discount Applied`, `Promo Code Used`

---

## ⚙️ Data Preprocessing & Feature Engineering
* **Missing Value Imputation:** Handled missing entries in `Review Rating` (37 null values) using appropriate statistical imputation (median/mean by product category).
* **Feature Engineering:**
  * Created `Age Group` bins (e.g., *Young Adult, Middle-Aged, Senior*) for demographic segmentation.
  * Derived `Customer Value Tier` based on `Purchase Amount (USD)` and `Previous Purchases`.
  * Standardized categorical variables and boolean indicators (`Discount Applied`, `Promo Code Used`).

---

## 🛠️ Tech Stack & Workflow
* **Python (Pandas, NumPy, Matplotlib, Seaborn):** Data cleaning, missing value handling, feature engineering, and exploratory data analysis (EDA).
* **SQL:** Relational data querying, cohort analysis, customer lifetime metrics, and category-level aggregations.
* **Power BI:** Interactive multi-page dashboard with dynamic filters for sales KPIs, category performance, and demographic breakdowns.
* **PowerPoint:** Executive slide deck presenting insights, data visualizations, and strategic business takeaways.
<img src="C:\Users\ankit\Pictures\Screenshots\Screenshot 2026-08-28 210256.png" alt="Description of photo" width="400">

---

## 🔍 Key Insights & Analysis Areas
* **Demographics & Revenue:** Identifying top spending age groups and gender distributions across product categories.
* **Subscription Impact:** Evaluating how subscription status influences order value, purchase frequency, and loyalty.
* **Promotional Effectiveness:** Measuring conversion rates and average order values when discounts and promo codes are applied.
* **Category & Seasonal Trends:** Highlighting peak demand seasons, top colors/sizes, and leading revenue-generating items.
* **Customer Satisfaction:** Assessing review ratings across shipping methods, categories, and payment types.

---

## 📁 Repository Structure
```text
├── data/
│   ├── raw/                        # Original dataset (3,900 records)
│   └── processed/                  # Cleaned dataset with new engineered features
├── notebooks/                      # Jupyter Notebooks (EDA, Data Cleaning & Feature Engineering)
├── sql/                            # SQL business queries & segmentation scripts
├── dashboard/                      # Power BI (.pbix) file & dashboard screenshots
├── presentation/                   # Executive PPT summary report
└── README.md                       # Project documentation
