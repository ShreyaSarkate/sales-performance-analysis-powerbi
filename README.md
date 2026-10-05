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
