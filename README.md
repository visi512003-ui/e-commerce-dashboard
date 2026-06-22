E-Commerce Sales Analytics Dashboard
Project Overview

This project analyzes three years of e-commerce sales data (2022–2024) to identify business trends, revenue drivers, profitability patterns, and regional performance.

The dashboard provides interactive visualizations and actionable insights to support data-driven decision-making.

Business Problem

Organizations generate large amounts of sales data but often struggle to extract meaningful insights.

This project answers key business questions:

Which product categories generate the most revenue?
Which regions perform best?
How has revenue changed over time?
What are the most profitable products?
Which business areas require improvement?
Tools & Technologies
Programming
Python
SQL
Libraries
Pandas
NumPy
Matplotlib
Seaborn
Visualization
Chart.js
HTML/CSS
Other Tools
Jupyter Notebook
PowerPoint
Dataset Information
Total Orders: 3,500
Time Period: 2022–2024
Regions: North, South, East, West
Product Categories:
Electronics
Accessories
Office
Data Cleaning Process

The dataset was cleaned using Python and Pandas.

Steps Performed
Removed duplicate records
Handled missing values
Standardized category names
Converted date fields
Validated numerical columns
Created derived metrics
Exploratory Data Analysis

Key metrics analyzed:

Revenue
Profit
Profit Margin
Order Volume
Average Order Value
Regional Performance
Category Performance
Dashboard Features
KPI Cards
Total Revenue
Total Profit
Total Orders
Average Order Value
Top Product
Visualizations
Monthly Revenue Trend
Profit Trend
Revenue by Category
Revenue by Region
Year-over-Year Comparison
Profit Margin Analysis
Top Product Analysis
Region vs Category Analysis
Key Insights
Revenue
Total Revenue: $10.67M
Profit
Total Profit: $1.84M
Top Category
Electronics generated approximately 50% of total revenue.
Top Product
Camera generated $1.18M in sales.
Best Region
West region contributed $2.84M in revenue.
Growth
Revenue increased by 16.3% from 2022 to 2023.
Strategic Recommendations
Expand Electronics Portfolio

Camera and Monitor products contribute significantly to revenue.

Improve North Region Performance

Targeted campaigns could reduce the performance gap.

Investigate Revenue Decline

A 4.3% decline in 2024 indicates a need for deeper analysis.

Expand Office Category

Adding more products could diversify revenue streams.

Project Screenshots

<img width="1918" height="715" alt="Screenshot 2026-05-26 172731" src="https://github.com/user-attachments/assets/8c72b178-4c2a-45ec-8555-0f9021ae4a93" />

Future Improvements
Power BI Dashboard
Automated ETL Pipeline
Sales Forecasting Model
Customer Segmentation
Interactive Filters
Author

Vipul Singh

LinkedIn: https://www.linkedin.com/in/vipul-singh34/

GitHub: https://github.com/visi512003-ui

requirements.txt

pandas
numpy
matplotlib
seaborn
jupyter
openpyxl

-- Total Revenue

SELECT
SUM(sales) AS total_revenue
FROM ecommerce_sales;

-- Revenue by Region--

SELECT
region,
SUM(sales) AS revenue
FROM ecommerce_sales
GROUP BY region
ORDER BY revenue DESC;

-- Top Products --

SELECT
product_name,
SUM(sales) AS revenue
FROM ecommerce_sales
GROUP BY product_name
ORDER BY revenue DESC
LIMIT 10;
