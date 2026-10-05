# 📊 Sales Performance Analysis Dashboard | Power BI

## 📌 Project Overview

This project is an interactive Sales Performance Analysis Dashboard developed using Microsoft Power BI.

The dashboard provides a visual overview of sales performance, profitability, orders, products, regions, customer types, and payment methods.

## 🎯 Project Objectives

- Analyze overall sales performance
- Track total sales and profit
- Monitor profit margin
- Analyze total orders and average order value
- Identify sales trends over time
- Compare sales performance across regions
- Analyze product performance
- Understand customer segments
- Analyze payment methods

## 🛠️ Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Excel
- Data Modeling

## 📊 Key KPIs

The dashboard includes the following key performance indicators:

- Total Sales
- Total Profit
- Profit Margin %
- Total Orders
- Average Order Value

## 🔄 Data Preparation

Power Query was used for data preparation and transformation, including:

- Data cleaning
- Data type conversion
- Header transformation
- Data validation
- Preparing numerical and date fields

A Calendar table was created using the minimum and maximum dates from the Sales table to support time-based analysis.

## 🧮 DAX Measures

The following DAX measures were created:

### Total Sales

```DAX
Total Sales = SUM('Sales'[Total Sales])

Total Profit
Total Profit = SUM('Sales'[Profit])

Profit Margin %
Profit Margin % =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)

Total Orders
Total Orders = DISTINCTCOUNT('Sales'[OrderID])

Average Order Value
Average Order Value =
DIVIDE(
    [Total Sales],
    [Total Orders],
    0
)

📈 Dashboard Features
- KPI Cards
- Sales Trend Analysis
- Regional Sales Analysis
- Product Analysis
- Customer Type Analysis
- Payment Method Analysis
- Interactive Filters
- Time-based Analysis

💡 Business Insights
The dashboard can be used to understand:
- Overall revenue and profitability
- Sales performance across regions
- Product-level sales performance
- Customer segment contribution
- Sales trends over time
- Average revenue generated per order

📷 Dashboard Preview
<img width="1920" height="1019" alt="Power BI Desktop 05-10-2026 16_39_01" src="https://github.com/user-attachments/assets/326c686b-64e1-4d3b-a49d-dc36486b12ca" />

 
📚 Learning Reference
This project was developed as a hands-on Power BI learning project using the following tutorial as a reference:
YouTube Tutorial:
https://youtu.be/v71YI0sm-TI

The project was implemented while learning Power Query, DAX, data modeling, Calendar tables, KPI creation, and Power BI visualization techniques.

~Shreya Sarkate
BE Computer Engineering
