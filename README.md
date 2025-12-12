# 📊 **Customer Shopping Behavior Analysis – Data Analytics Project**

<img width="1289" height="708" alt="image" src="https://github.com/user-attachments/assets/e26e2c10-d77a-42e9-8196-e96f77bc7306" />


## ⭐ **1. Overview**

This project provides an end-to-end analysis of **customer shopping behavior** using a dataset of 3,900 transactions across multiple product categories. The goal is to uncover insights on **spending patterns, customer segments, product preferences, subscription behavior, and seasonal trends**, and present the findings through a **Power BI dashboard** and **summary report**.

The workflow includes:
✔ Loading and exploring the data in Python
✔ Cleaning and transforming the dataset
✔ Running analytical SQL queries in PostgreSQL
✔ Building an interactive Power BI dashboard
✔ Creating a final report and presentation using Gamma


## 📁 2. Dataset

* **Rows:** 3,900
* **Columns:** 18
* **Data Includes:**

  * Customer demographics: age, gender, location, subscription status
  * Purchase details: item purchased, category, purchase amount, season, size, color
  * Behavioral attributes: discount applied, promo code used, previous purchases, frequency of purchases, review rating, shipping type
* **Missing Values:** 37 missing review ratings were identified and imputed during cleaning


## 🛠️ 3. Tools Used

* **Python:** pandas, numpy, matplotlib, seaborn
* **PostgreSQL:** pgAdmin, SQLAlchemy, psycopg2
* **Power BI:** Dashboard design & visual analytics
* **Jupyter Notebook:** Development environment


## 🔍 4. Project Steps

### A. Data Preparation & EDA (Python)

* Loaded the dataset using pandas
* Reviewed structure and summary statistics using `.info()` and `.describe()`
* Handled missing values by imputing review ratings with **median rating per category**
* Standardized column names into snake_case for clarity
* Created engineered features like:

  * `age_group` (binned age ranges)
  * `purchase_frequency_days`
* Removed redundant fields such as `promo_code_used` after validation

### **B. SQL Analysis in PostgreSQL**

After loading the cleaned DataFrame into PostgreSQL, several business questions were answered through SQL queries, including:

* Revenue by gender
* High-spending customers who used discounts
* Top-rated products
* Shipping type comparison
* Subscribers vs non-subscribers
* Products most dependent on discounts
* Customer segmentation (New, Returning, Loyal)
* Top 3 most purchased products within each category (via window functions)
* Revenue contribution by age group

### **C. Power BI Dashboard**

An interactive dashboard was built to visualize:

* Total customers
* Average purchase amount
* Average review rating
* Subscription analysis
* Revenue by category
* Sales by age group
* Impact of shipping type
* Category-wise and product-wise trends

The dashboard consolidates key KPIs and supports actionable decision-making.

## 📈 **5. Key Results**

Based on the analysis:

* **Male customers generated higher revenue** compared to females
* Several customers use discounts yet still spend above the average amount
* Gloves, Sandals, Boots, Hats, and Skirts ranked as **top-rated products**
* Express shipping customers spend more than standard shipping users
* Most customers fall into the **Loyal** segment
* Hats, Sneakers, Coats, and Sweaters show the **highest discount dependency**
* Accessories and Clothing categories have the **highest-purchased products**
* Young Adults contribute the highest revenue among age groups

## 🏁 8. Conclusion

This project demonstrates a complete end-to-end data analytics workflow—from data loading and cleaning in Python, to SQL-based business analysis in PostgreSQL, to visual analytics in Power BI and final reporting through Gamma. The insights uncovered help understand customer behavior across demographics, purchase patterns, discount dependence, and subscription trends.

The interactive dashboard and analytical findings can support decisions around **marketing strategy, customer retention, product performance, and revenue optimization**. Overall, the project reflects strong skills in **Python, SQL, data storytelling, and BI visualization**, suitable for real-world business analytics scenarios.


## 📊 9. Power BI Dashboard

Access the interactive dashboard here:

👉 **Power BI Dashboard:** *[https://app.powerbi.com/view?r=eyJrIjoiNTRjMGU2NjYtYmM1My00YzI5LTljNTktNjAwN2M0NjAzZTU4IiwidCI6ImUxNGU3M2ViLTUyNTEtNDM4OC04ZDY3LThmOWYyZTJkNWE0NiIsImMiOjEwfQ%3D%3D]*
