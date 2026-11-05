# Customer Analytics Dashboard | Power BI

## Project Overview

This project presents an interactive Customer Analytics Dashboard developed using Microsoft Power BI. It focuses on analyzing customer demographics, spending behavior, and key business performance indicators.

The dashboard transforms customer data into meaningful insights through interactive visualizations, KPI tracking, and customer segmentation.

## Dashboard Preview

<img width="1171" height="657" alt="Ekran görüntüsü 2026-11-05 160032" src="https://github.com/user-attachments/assets/d2bae7ff-a6b2-4bb1-be3c-aa393ee2998c" />


## Key Features

- Customer overview and KPI tracking
- Total customer and spending analysis
- Average customer spending analysis
- Customer age distribution
- Spending analysis by city
- Interactive city filtering
- Customer segmentation by age groups

## Tools & Technologies

- Microsoft Power BI
- DAX (Data Analysis Expressions)
- Data Modeling
- Data Visualization
- Microsoft Excel

## Key DAX Measures

**Total Customers**
```dax
Total Customers = DISTINCTCOUNT(customers[Customer_ID])
```

**Total Spending**
```dax
Total Spending = SUM(customers[Annual_Spending])
```

**Average Spending**
```dax
Avg Spending = AVERAGE(customers[Annual_Spending])
```

**Average Age**
```dax
Avg Age = AVERAGE(customers[Age])
```

## Customer Segmentation

Customers are categorized into age groups using a calculated column created with DAX.

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

## Dashboard Insights

The dashboard enables users to:

- Explore customer distribution across different cities.
- Compare spending behavior across customer groups.
- Analyze customer demographics by age.
- Monitor key performance indicators.
- Interact with data through dashboard filters.

## Project Files

| File | Description |
|---|---|
| `customer-analytics-dashboard.pbix` | Power BI dashboard file |
| `dashboard-preview.png` | Dashboard preview image |

## Project Objective

The objective of this project is to demonstrate practical skills in business intelligence, data analysis, data modeling, DAX calculations, and interactive dashboard development.

This project is part of my portfolio in Management Information Systems and Data Analytics.
