Customer Shopping Behavior Analysis 🛒📊
Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The objective is to extract actionable business insights related to spending patterns, customer segmentation, product performance, and subscription behavior using Python, SQL (MySQL), and Power BI.

This is an end-to-end data analytics project covering data cleaning, feature engineering, database integration, SQL-based business analysis, and dashboard visualization.

Dataset Summary

Total Rows: 3,900

Total Columns: 18

Key Features

Customer Demographics:
age, gender, location, subscription_status

Purchase Details:
item_purchased, category, purchase_amount, season, size, color

Shopping Behavior:
discount_applied, promo_code_used, previous_purchases,
frequency_of_purchases, review_rating, shipping_type

Missing Data:

37 missing values in the review_rating column

Tools & Technologies

Python: pandas, numpy

Database: MySQL

Visualization: Power BI

Environment: Jupyter Notebook / Google Colab

Data Cleaning & Preparation (Python)

Key preprocessing steps performed in Python:

Data Loading: Imported dataset using pandas

Initial Exploration:

df.info() for structure and data types

df.describe() for statistical overview

Missing Value Handling:

Imputed missing review_rating values using the median rating of each product category

Column Standardization:

Converted column names to snake_case

Feature Engineering:

Created age_group by binning customer ages

Created purchase_frequency_days from purchase behavior data

Data Consistency Check:

Identified redundancy between discount_applied and promo_code_used

Dropped promo_code_used

Database Integration:

Connected Python to MySQL

Loaded cleaned dataset into a relational table for SQL analysis

Business Analysis (SQL – MySQL)

SQL queries were written to answer real business questions:

Revenue by Gender
→ Compared total revenue between male and female customers

High-Spending Discount Users
→ Customers using discounts but spending above the average purchase amount

Top 5 Products by Rating
→ Products with the highest average review ratings

Shipping Type Comparison
→ Average purchase amount for Standard vs Express shipping

Subscribers vs Non-Subscribers
→ Average spend and total revenue comparison

Discount-Dependent Products
→ Top 5 products with the highest percentage of discounted purchases

Customer Segmentation
→ Classified customers into New, Returning, and Loyal based on purchase history

Top 3 Products per Category
→ Most purchased products within each category

Repeat Buyers & Subscriptions
→ Checked if customers with more than 5 purchases are more likely to subscribe

Revenue by Age Group
→ Total revenue contribution of each age group

Power BI Dashboard

An interactive Power BI dashboard was built to visualize key insights:

Revenue breakdown by gender and age group

Subscriber vs non-subscriber performance

Top products and categories

Shipping type impact on spending

Customer segmentation overview

The dashboard enables business stakeholders to quickly identify trends and make data-driven decisions.

Key Business Insights

Subscribers generate higher average revenue than non-subscribers

Loyal customers contribute a disproportionate share of total revenue

Certain products are highly discount-dependent, impacting margins

Express shipping users tend to have higher purchase values

Specific age groups drive the majority of revenue

Business Recommendations

Boost Subscriptions: Offer exclusive benefits to convert repeat buyers

Customer Loyalty Programs: Incentivize customers to move into the “Loyal” segment

Optimize Discount Strategy: Balance revenue growth with profit margins

Product Positioning: Promote top-rated and best-selling products

Targeted Marketing: Focus campaigns on high-revenue age groups and express-shipping users
