# Coffee---Sales---Analysis---Dashboard-
☕ Coffee Sales Performance Analysis

1. Project Overview

This project is an end-to-end data analytics case study focused on analyzing coffee shop sales data from a fast-growing café chain operating in Lower Manhattan, Hell’s Kitchen, and Astoria (USA).
The goal of this project is to transform raw transactional data into actionable business insights using Excel and Power BI, and present them through an interactive dashboard suitable for data-driven decision-making.

2. Dataset Information

- Source: Kaggle – Coffee Shop Sales Dataset
- Time Period: January 2023 – June 2023
- Rows: 149,116
- Columns: 11 (cleaned to 10)
  
3. Business Objectives

The analysis was conducted to evaluate performance across 7 key KPIs:
- Total Revenue
- Average Order Value (AOV)
- Revenue by Product Category
- Revenue by Store Location
- Top 5 Selling Products
- Monthly Revenue Trends
- Average Sales per Hour
  
Key Columns:
- Transaction ID
- Transaction Date & Time
- Transaction Quantity
- Store Location
- Product Category & Type
- Unit Price

4. Data Cleaning & Preparation

Data preparation was done in MS Excel:
- Removed unnecessary column (product_detail)
- Standardized date formats
- Applied currency formatting
- Verified data consistency and completeness

5. Excel Analysis

Key Excel techniques used:
- SUMPRODUCT for Total Revenue calculation
- Pivot Tables & Charts for category, location, and product analysis
- VLOOKUP & XLOOKUP for product-level insights

Time-based analysis by extracting hours from transaction time:
Key Excel Insights:
- Total Revenue: $698,812.33
- Average Order Value (AOV): $4.69
- Top Product Category: Coffee (≈39% of total revenue)
- Top Location: Hell’s Kitchen (≈34% of revenue)
- Peak Hour: 8 PM 

6. Power BI Dashboard

The cleaned dataset was imported into Power BI for advanced visualization.

Features:
- Interactive KPI cards
- Dynamic filters (location, product category, month)
- Coffee-themed color palette
- Clean and business-focused layout

Key DAX Measures:
- Total Revenue = SUMX(Transactions, Transactions[transaction_qty] * Transactions[unit_price])
- AOV = [Total Revenue] / DISTINCTCOUNT(Transactions[transaction_id])
- Hour = HOUR(Transactions[transaction_time])
- Avg Sales per Hour = AVERAGEX(VALUES(Transactions[Hour]), CALCULATE([Total Revenue]))

7. Key Insights
   
Overall Performance:
- Achieved ~$698.8K revenue in 6 months
- Revenue doubled from January ($82K) to June ($166K)
  
Location Analysis:
- Revenue distribution is well-balanced across all three locations
- Indicates strong brand presence and customer loyalty
  
Product Analysis:
- Coffee and Tea contribute over 65% of total revenue
- Low-performing items like packaged chocolate need re-evaluation

Time-Based Insights:
- Morning hours (8–10 AM) are the busiest
- Afternoon and evening hours show growth potential.

8. Strategic Recommendations

- Promote high-margin products through loyalty programs
- Introduce “Happy Hour” or combo offers during non-peak hours
- Launch seasonal products to maintain customer engagement
- Use localized promotions to enhance store-level performance

9. Tools & Technologies Used

- MS Excel – Data cleaning, analysis, formulas
- Microsoft Power BI – Dashboard & DAX measures
- DAX – KPI calculations
- Data Visualization & Business Analysis

Conclusion :
This project demonstrates how data analytics can drive business decisions by identifying revenue drivers, customer behavior, and growth opportunities.



