# Customer Analytics Dashboard | Power BI

## Project Overview

An interactive Customer Analytics Dashboard developed using Microsoft Power BI to analyze customer demographics, spending behavior, and key business performance indicators.

The project demonstrates practical skills in data analysis, business intelligence, data modeling, and dashboard development.

## Dashboard Preview

<img width="1171" height="657" alt="Ekran görüntüsü 2026-11-05 160032" src="https://github.com/user-attachments/assets/c750cefb-d9d0-4e01-9809-a0a71aecd464" />


## Key Features

- Total customer count
- Total and average customer spending
- Average customer age
- Customer distribution by age group
- Customer spending analysis by city
- Interactive city filter
- KPI tracking and data visualization

## Tools & Technologies

- Microsoft Power BI
- DAX (Data Analysis Expressions)
- Data Modeling
- Data Visualization
- Data Analysis

## DAX Measures

```dax
Total Customers = DISTINCTCOUNT(customers[Customer_ID])

Total Spending = SUM(customers[Annual_Spending])

Avg Spending = AVERAGE(customers[Annual_Spending])

Avg Age = AVERAGE(customers[Age])
```

## Customer Segmentation

An age group calculated column is used to categorize customers.

```dax
Age Group =
SWITCH(
    TRUE(),
    customers[Age] < 25, "18-24",
    customers[Age] < 35, "25-34",
    customers[Age] < 45, "35-44",
    customers[Age] < 55, "45-54",
    "55+"
)
```

## Data Model

The analysis uses customer data containing:

- Customer_ID
- Age
- City
- Annual_Spending

## Project Files

- `customer-analytics-dashboard.pbix` – Power BI dashboard file
- `dashboard-preview.png` – Dashboard preview image

## Project Objective

The objective of this project is to transform customer data into meaningful business insights through interactive visualizations, customer segmentation, and KPI tracking.
