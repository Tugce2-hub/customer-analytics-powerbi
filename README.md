# Customer Analytics Dashboard | Power BI

## Project Overview
This project presents an interactive Customer Analytics Dashboard developed using Microsoft Power BI. It focuses on customer demographics, spending behavior, and key business performance indicators.

## Dashboard Preview

## Dashboard Preview

![Customer Analytics Dashboard](dashboard-preview.png)

## Key Features
- Total customer count
- Total and average customer spending
- Average customer age
- Customer distribution by age group
- Customer spending analysis by city
- Interactive city filter

## Tools & Technologies
- Microsoft Power BI
- DAX
- Data Visualization
- Data Analysis

## DAX Measures

```dax
Total Customers = DISTINCTCOUNT(customers[Customer_ID])

Total Spending = SUM(customers[Annual_Spending])

Avg Spending = AVERAGE(customers[Annual_Spending])

Avg Age = AVERAGE(customers[Age])
```

## Data Model
The analysis uses customer data containing fields such as:
- Customer_ID
- Age
- City
- Annual_Spending

An additional calculated column, `Age Group`, categorizes customers into age ranges.

## Project Files
- `customer-analytics-dashboard.pbix` – Power BI dashboard file.
- `dashboard-preview.png` – Dashboard screenshot.

## Project Objective
The objective of this project is to transform customer data into meaningful business insights through interactive visualizations and KPI tracking.
