# WalmartsalesAnalysis
Project Overview
This project focuses on analyzing Walmart sales data to gain insights into branch performance, product sales trends, and customer behavior. By exploring historical sales data, we aim to identify key factors affecting sales across different Walmart branches and suggest improvements to sales strategies. The dataset used in this analysis is from the Kaggle Walmart Sales Forecasting Competition.

The competition challenges participants to project sales for various departments across 45 Walmart stores, with factors such as holiday markdowns adding complexity to the predictions.

Objectives
The main goal of this project is to analyze Walmart’s sales data to understand:

The performance of different product lines.
The factors influencing customer purchasing decisions.
Sales trends across branches and product lines.
Strategies to optimize and improve sales performance.
Dataset Information
The dataset contains sales transactions from three Walmart branches located in Mandalay, Yangon, and Naypyitaw. It includes 17 columns and 1,000 rows, with the following details:

Column	Description	Data Type
invoice_id	Invoice for the sales transaction	VARCHAR(30)
branch	Branch where the sale was made	VARCHAR(5)
city	Location of the branch	VARCHAR(30)
customer_type	Type of customer	VARCHAR(30)
gender	Gender of the customer	VARCHAR(10)
product_line	Product line of the sold item	VARCHAR(100)
unit_price	Price of each product	DECIMAL(10, 2)
quantity	Number of products sold	INT
VAT	Tax on the purchase	FLOAT(6, 4)
total	Total cost of the purchase	DECIMAL(10, 2)
date	Date of purchase	DATE
time	Time of purchase	TIMESTAMP
payment_method	Payment method	VARCHAR(30)
cogs	Cost of goods sold	DECIMAL(10, 2)
gross_margin_percentage	Gross margin percentage	FLOAT(11, 9)
gross_income	Gross income from the sale	DECIMAL(10, 2)
rating	Customer rating	FLOAT(2, 1)
Project Workflow
1. Data Wrangling
Data Cleaning: Inspect the dataset for missing values and null data. Handle missing/null values appropriately.
Database Creation: Set up a database, create tables, and ensure fields are marked as NOT NULL where required.
Feature Engineering: Create new columns such as time_of_day, day_name, and month_name to analyze sales trends based on different times of the day, days of the week, and months.
2. Exploratory Data Analysis (EDA)
Analyze key performance indicators and trends in sales data.
Address key business questions related to product performance, customer behavior, and branch sales.
Business Questions
Product Analysis
How many unique product lines are in the dataset?
Which product line is the most popular?
What payment method is most commonly used?
Which product line generates the most revenue?
What is the most profitable month based on total revenue and cost of goods sold (COGS)?
Sales Analysis
What are the sales patterns throughout the day and week?
Which branch has sold more products than the average?
Which customer type generates the most revenue?
Which city has the highest tax (VAT) percentage?
Customer Analysis
What is the gender distribution of customers per branch?
Which customer type makes the most purchases?
Which day of the week receives the highest ratings?
Revenue and Profit Calculations
Cost of Goods Sold (COGS):

COGS
=
unit_price
×
quantity
COGS=unit_price×quantity
VAT Calculation:

VAT
=
5
%
×
COGS
VAT=5%×COGS
Total Sale (Gross Sales):

total
=
VAT
+
COGS
total=VAT+COGS
Gross Profit:

gross_income
=
total
−
COGS
gross_income=total−COGS
Gross Margin Percentage:

Gross Margin
=
gross_income
total revenue
Gross Margin= 
total revenue
gross_income
​
 
Example Calculation:
For a sale where:

Unit Price = $45.79

Quantity = 7

COGS = 
45.79
×
7
=
320.53
45.79×7=320.53

VAT = 
5
%
×
320.53
=
16.03
5%×320.53=16.03

Total = 
320.53
+
16.03
=
336.56
320.53+16.03=336.56

Gross Margin Percentage = 
16.03
336.56
≈
4.76
%
336.56
16.03
​
 ≈4.76%

Conclusion
The Walmart Sales Data Analysis project provides insights into product performance, customer behavior, and sales trends across branches. By answering key business questions and conducting detailed revenue and profit analyses, the project aims to inform data-driven strategies to optimize sales and improve overall business operations.
