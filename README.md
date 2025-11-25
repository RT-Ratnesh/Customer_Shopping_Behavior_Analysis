# Customer Shopping Behavior Analysis

End-to-end retail analytics project using **Python**, **SQL**, and **Power BI** to understand customer shopping behavior and generate business-ready insights.

---

## Overview

This project simulates a real-world analytics workflow for a retail business:

- Clean and explore a **customer shopping behavior** dataset in Python  
- Load the refined data into a SQL database for **business questioning**
- Build a **Power BI dashboard** for stakeholders
- Summarize **key insights and recommendations** in a report and presentation

It is designed to showcase practical skills that recruiters look for in data roles:
**data cleaning, feature engineering, SQL analysis, dashboarding, and storytelling.** 

---

## Dataset

**File:** `customer_shopping_behavior.csv` 

The dataset contains around **3,900 retail transactions** and includes:

- **Customer demographics** – age, gender, location  
- **Product details** – item purchased, category, rating  
- **Shopping behavior** – discounts, promo code usage, purchase frequency  
- **Purchase details** – purchase amount, shipping type, subscription status  

This dataset is ideal for answering questions such as:

- Which customer segments generate the most revenue?
- How do discounts and promo codes influence spending?
- Which products and categories perform best?
- How do subscribers differ from non-subscribers in terms of value? 

---

## Tools

This project uses:

- **Python (Jupyter Notebook)** – data loading, cleaning, feature engineering, EDA  
  - Main file: `customer_shopping_behavior_analysis.ipynb` 
- **SQL (any relational database – MySQL/PostgreSQL/SQL Server)** – business analysis  
  - Main file: `customer_behavior_business_sql_queries.sql` 
- **Power BI** – interactive dashboard  
  - Main file: `customer_behavior_dashboard.pbix` 
- **Documentation** – business and insight communication  
  - `Business Problem Document.pdf`  
  - `Customer Shopping Behavior Analysis.pdf`  
  - `Customer-Shopping-Behavior-Analysis.pptx`

---

## Project Steps

### 1. Exploratory Data Analysis in Python

In `customer_shopping_behavior_analysis.ipynb` you will find:

- Loading `customer_shopping_behavior.csv`
- Checking data types, missing values, and distributions
- Handling missing review ratings and other data quality issues
- Standardizing column names and creating derived fields such as:
  - Age groups (e.g., young adults, adults, middle-aged, seniors)
  - Purchase frequency and customer segment tags (new/returning/loyal) 

The final cleaned dataframe is prepared for loading into SQL.

---

### 2. Loading Data into SQL

Using Python + a database connector (e.g., SQLAlchemy / native driver), the cleaned dataset is pushed into a relational database table, typically named something like `customer_shopping_behavior`.

Steps (high level):

1. Create a new database (e.g., `customer_analytics`)
2. Create a table schema compatible with the CSV columns
3. Use the notebook to insert/load data into the table 

---

### 3. SQL Business Analysis

The file `customer_behavior_business_sql_queries.sql` contains queries that answer real business questions, such as:

- **Revenue by gender**  
- **High-spending customers who still use discounts**
- **Top products by average review rating**
- **Standard vs. express shipping behavior and revenue**
- **Subscribers vs. non-subscribers – average spend and total revenue**
- **Products most dependent on discounts**
- **Customer segmentation** into New, Returning, Loyal
- **Top 3 products within each category**
- **Revenue contribution by age group**

These queries demonstrate how SQL is used to support strategic decisions in marketing, pricing, and retention.

---

### 4. Power BI Dashboard

The dashboard in `customer_behavior_dashboard.pbix` brings together the cleaned data and SQL outputs into an **executive-friendly view**. 

Typical views include:

- **Customer Demographics**
  - Age group breakdown  
  - Gender distribution  
  - Subscribers vs. non-subscribers  

- **Revenue & Sales Performance**
  - Total revenue and transaction count  
  - Revenue by age group, gender, and segment  
  - Seasonal or time-based trends  

- **Product Analytics**
  - Best-selling products and categories  
  - Top-rated products  
  - Discount-driven products  

- **Behavior & Segmentation**
  - New vs. Returning vs. Loyal customers  
  - Purchase frequency  
  - Impact of shipping type and discounts on revenue  

---

## Key Results & Insights (Summary)

The exact numbers will depend on your runs, but the analysis typically highlights patterns such as:

- **High-value segments**  
  - Certain age groups (e.g., young adults/adults) contribute a large share of revenue  
  - Loyal customers (with many previous purchases) are especially valuable  

- **Pricing & discount behavior**
  - Some customers spend above-average amounts even when using discounts  
  - A subset of products is heavily discount-dependent  

- **Shipping & subscription**
  - Express shipping is often associated with higher purchase amounts  
  - Subscription or membership status correlates with higher engagement and frequency  

- **Product performance**
  - A small set of top-rated and top-selling products drives a meaningful portion of revenue  

These insights translate directly into **actionable recommendations** for marketing, pricing, and customer retention strategies.

---

## 📜 License

MIT


