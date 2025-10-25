# 🛍️ Customer Shopping Behavior Analysis

## 📘 Project Overview
This project analyzes **customer shopping behavior** using transactional data from **3,900 purchases** across multiple product categories.  
The goal is to uncover **insights into spending patterns, customer segments, product preferences, and subscription behavior** to guide **strategic business decisions**.

---

## 📊 Dataset Summary
- **Total Rows:** 3,900  
- **Total Columns:** 18  
- **Key Features:**
  - Customer Demographics: `Age`, `Gender`, `Location`, `Subscription Status`
  - Purchase Details: `Item Purchased`, `Category`, `Purchase Amount`, `Season`, `Size`, `Color`
  - Shopping Behavior: `Discount Applied`, `Promo Code Used`, `Previous Purchases`, `Review Rating`, `Shipping Type`
- **Missing Data:** 37 missing values in `Review Rating` column (imputed with median per category)

---

## 🐍 Data Preparation & Exploration (Python)
Performed in **Python** using libraries such as `pandas`, `numpy`, and `matplotlib`.

**Steps:**
1. **Data Loading & Exploration** – Imported dataset and checked structure using `df.info()` and `df.describe()`.
2. **Missing Data Handling** – Imputed missing review ratings using the median per category.
3. **Column Standardization** – Converted column names to `snake_case`.
4. **Feature Engineering:**
   - Created `age_group` column by binning age ranges.
   - Created `purchase_frequency_days` column from purchase timestamps.
5. **Data Consistency Check** – Removed redundant `promo_code_used` column.
6. **Database Integration** – Loaded cleaned data into **PostgreSQL** for advanced SQL queries.

---

## 🧮 Data Analysis (SQL)
Key insights were generated from SQL queries on the cleaned dataset:

| # | Analysis Focus | Key Findings |
|---|----------------|--------------|
| 1 | **Revenue by Gender** | Male customers generate 68% of total revenue. |
| 2 | **High-Spending Discount Users** | 21.5% of customers use discounts yet spend above average. |
| 3 | **Top 5 Products by Rating** | Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78). |
| 4 | **Shipping Type Comparison** | Express shipping correlates with higher spend. |
| 5 | **Subscribers vs Non-Subscribers** | Similar average spend; opportunity to convert repeat buyers. |
| 6 | **Discount-Dependent Products** | Identified products most reliant on discounts. |
| 7 | **Customer Segmentation** | 80% loyal customers – strong retention potential. |
| 8 | **Revenue by Age Group** | Identified high-revenue age segments for marketing focus. |

---

## 📈 Dashboard (Power BI)
A **Power BI dashboard** was created to visualize:
- Revenue distribution by gender, age, and location  
- Product ratings and performance  
- Subscription impact on sales  
- Discount and loyalty segmentation  

This enables **real-time decision-making** and **data-driven strategy** refinement.

---

## 💡 Business Recommendations
1. **Boost Subscriptions:** Promote exclusive benefits to convert repeat buyers.  
2. **Customer Loyalty Programs:** Reward frequent customers to strengthen retention.  
3. **Review Discount Policy:** Optimize discount strategies to balance margin and volume.  
4. **Product Positioning:** Highlight top-rated and best-selling items in campaigns.  
5. **Targeted Marketing:** Focus on high-revenue age groups and express-shipping users.

---

## 🧰 Tools & Technologies
- **Languages:** Python, SQL  
- **Libraries:** pandas, numpy, matplotlib, seaborn  
- **Database:** PostgreSQL  
- **Visualization:** Power BI  
- **Environment:** Jupyter Notebook  

---


## 👩‍💻 Author
**Project Lead:** [Nakul]  
**Contact:** [ashubagri039@gmail.com]  
**LinkedIn:** https://www.linkedin.com/in/nakul-bagri-a9b239285/ 

---

⭐ *If you found this project insightful, don’t forget to star the repo!*
