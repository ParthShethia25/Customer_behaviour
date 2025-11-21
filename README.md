
# 🛒 Customer Shopping Behavior Analysis

A Data Analytics Project using **Python**, **PostgreSQL**, and **Power BI**

## 📌 Project Overview

This project investigates customer shopping behavior using 3,900 transactional records.
The goal is to extract insights about spending patterns, product preferences, customer segmentation, and subscription trends to support business decision-making.

---

## 📂 Dataset Summary

* **Rows:** 3,900
* **Columns:** 18
* **Key Features:**

  * Customer demographics (Age, Gender, Location, Subscription Status)
  * Purchase details (Item Purchased, Category, Purchase Amount, Season, Size, Color)
  * Behavioral attributes (Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type)
* **Missing Data:** Review Rating column had 37 missing values

---

## 🧹 Data Preparation & Cleaning (Python)

Steps performed during preprocessing:

* Loaded dataset and explored structure using pandas
* Handled missing values by imputing category-wise median ratings
* Standardized all column names to snake_case
* Created new engineered features:

  * `age_group` (binned age ranges)
  * `purchase_frequency_days`
* Checked redundancy between discount-related fields and removed unnecessary columns
* Loaded cleaned dataset into PostgreSQL for deeper analytics

---

## 🗄️ SQL Analysis (PostgreSQL)

SQL queries were used to answer key business questions, including:

### ✔ Revenue by Gender

Analyzed which gender contributes more to overall revenue.

### ✔ High-Spending Discount Users

Identified customers who used discounts but still spent above the average purchase amount.

### ✔ Top 5 Products by Rating

Ranked products based on average customer review scores.

### ✔ Shipping Type Comparison

Compared average purchase amounts between standard and express shipping.

### ✔ Subscribers vs Non-Subscribers

Compared total customers, average spend, and total revenue of subscription vs non-subscription users.

### ✔ Discount-Dependent Products

Listed products most frequently bought with applied discounts.

### ✔ Customer Segmentation

Classified customers into:

* New
* Returning
* Loyal

### ✔ Top 3 Products per Category

Ranked the most purchased products in each category.

### ✔ Repeat Buyers & Subscriptions

Checked correlation between repeat purchase behavior and subscription likelihood.

### ✔ Revenue by Age Group

Calculated revenue contribution of each age group.

---

## 📊 Dashboard (Power BI)

A fully interactive Power BI dashboard was built to visualize:

* Number of customers
* Average purchase amount
* Average rating
* Revenue by category
* Revenue by subscription status
* Sales by age group
* Shipping preferences

---

## 💡 Business Recommendations

### ⭐ Boost Subscriptions

Promote exclusive benefits to increase subscriber count.

### ⭐ Strengthen Customer Loyalty Programs

Offer targeted rewards to convert returning customers into loyal customers.

### ⭐ Evaluate Discount Strategy

Optimize discount rules to maintain margin while boosting sales.

### ⭐ Highlight Best-Selling & Top-Rated Products

Use them in marketing campaigns for improved conversion.

### ⭐ Prioritize High-Value Segments

Focus on high-spending age groups and express-shipping customers.

---

## 🛠️ Tech Stack

* **Python** (Pandas)
* **PostgreSQL**
* **Power BI**
* **Kaggle Notebook**

---




