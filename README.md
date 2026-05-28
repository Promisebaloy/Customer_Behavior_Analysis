# Customer Shopping Behavior Analysis

## Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories. The goal is to uncover spending trends, customer preferences, subscription behavior, and purchasing patterns to support data-driven business decisions and marketing strategies.

The project combines:

* **Python** for data cleaning, preprocessing, and exploratory data analysis (EDA)
* **MySQL** for business-focused SQL analysis
* **Power BI** for dashboard visualization and reporting

---

# Dataset Summary

The dataset contains:

* **3,900 records**
* **18 variables**

### Features Included

* Customer demographics:

  * Age
  * Gender
  * Location
  * Subscription status

* Purchase information:

  * Item purchased
  * Product category
  * Purchase amount
  * Season
  * Size
  * Color

* Shopping behavior indicators:

  * Discounts applied
  * Promo code usage
  * Previous purchases
  * Purchase frequency
  * Review ratings
  * Shipping type

### Data Quality

* 37 missing values were identified in the `review_rating` column.

---

# Exploratory Data Analysis (EDA)

The analysis process started with Python-based data exploration and preprocessing.

## Steps Performed

* Imported and explored the dataset using **Pandas**
* Reviewed dataset structure with:

  ```python
  df.info()
  ```
* Examined sample records using:

  ```python
  df.head()
  ```
* Generated descriptive statistics using:

  ```python
  df.describe()
  ```
* Checked for missing values and inconsistencies

---

# Data Cleaning & Preparation

## Missing Value Handling

* Missing values in the `review_rating` column were filled using the median rating within each product category.

## Column Standardization

* Column names were converted into **snake_case** format for improved readability and consistency.

---

# Feature Engineering

Additional features were created to improve analysis:

* `age_group`

  * Grouped customers into age ranges

* `purchase_frequency_days`

  * Created to better analyze customer purchasing behavior over time

---

# Data Validation

A consistency check was conducted between:

* `discount_applied`
* `promo_code_used`

Since both variables contained overlapping information, the `promo_code_used` column was removed to simplify the dataset.

---

# Database Integration

After preprocessing:

* The cleaned dataset was connected to **MySQL** using Python
* The processed DataFrame was loaded into the database for SQL analysis

---

# SQL Business Analysis

The following business questions were explored using MySQL:

## 1. Revenue by Gender

Compared male and female customers to determine which group generated more revenue.

## 2. High-Spending Discount Users

Identified customers using discounts while still spending above the average purchase amount.

## 3. Top 5 Products by Rating

Determined the products with the highest average customer ratings.

## 4. Shipping Type Comparison

Compared average spending between Standard and Express shipping users.

## 5. Subscribers vs Non-Subscribers

Analyzed spending behavior and revenue contribution based on subscription status.

## 6. Discount-Dependent Products

Identified products most reliant on discounts to generate purchases.

## 7. Customer Segmentation

Segmented customers into:

* New
* Returning
* Loyal

## 8. Top 3 Products per Category

Identified the most purchased products within each category.

## 9. Repeat Buyers and Subscriptions

Examined whether repeat customers were more likely to subscribe.

## 10. Revenue by Age Group

Analyzed revenue contribution across different customer age groups.

---

# Power BI Dashboard

An interactive Power BI dashboard was developed to visualize:

* Customer behavior
* Spending trends
* Product performance
* Subscription analysis
* Revenue insights
* Customer segmentation

The dashboard makes it easier to explore insights and communicate business findings effectively.

---

# Business Recommendations

## Increase Subscription Engagement

Encourage subscriptions through:

* Loyalty rewards
* Exclusive discounts
* Early product access

## Strengthen Customer Loyalty Programs

Reward repeat purchases to move customers into the Loyal segment.

## Evaluate Discount Strategies

Optimize promotional campaigns while protecting profit margins.

## Improve Product Positioning

Promote top-rated and best-selling products more aggressively.

## Enhance Targeted Marketing

Focus marketing efforts on:

* High-revenue age groups
* Customers preferring express shipping

---

# Tools & Technologies

* Python
* Pandas
* NumPy
* MySQL
* Power BI
* Jupyter Notebook

---

# Project Objectives

* Understand customer purchasing behavior
* Identify high-value customer segments
* Analyze product performance
* Evaluate subscription effectiveness
* Support business decision-making with data insights

---

# Author

Promise Baloyi

