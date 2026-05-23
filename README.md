# End-to-End E-COMMERCE-SALES-ANALYSIS-USING-POWER-BI

## Project Overview

This project is an end-to-end Business Intelligence solution built using Power BI to analyze e-commerce sales performance, customer behavior, product trends, and profitability.

The objective of the project is to transform raw transactional data into meaningful business insights through data cleaning, modeling, DAX calculations, and interactive dashboard visualizations.

The dashboard helps stakeholders:
- Monitor sales performance
- Analyze profitability
- Identify high-performing products
- Understand customer behavior
- Track regional performance
- Evaluate shipping efficiency
- Support data-driven decision making

---

# Business Problem

E-commerce businesses generate large volumes of transactional data daily. Without proper analysis, it becomes difficult to:

- Identify profitable products and regions
- Track sales growth trends
- Understand customer purchasing behavior
- Measure operational efficiency
- Detect loss-making products
- Evaluate the impact of discounts on profit

This project addresses these challenges by building a comprehensive analytics dashboard in Power BI.

---

# Tools & Technologies Used

| Tool | Purpose |
|------|----------|
| Power BI | Dashboard development & visualization |
| Power Query | Data cleaning & transformation |
| DAX | KPI calculations & analytics |
| MySQL | Data querying & extraction |
| Excel | Initial dataset preparation |

---

# Dataset Description

The dataset contains e-commerce transactional data including:

- Orders
- Customers
- Products
- Sales
- Shipping details
---

# Data Model

The project follows a **Star Schema** data modeling approach.

## Fact Table
### FactSales
Contains transactional sales data.

### Key Columns
- Order ID
- Order Date
- Customer ID
- Product ID
- Sales
- Quantity
- Ship Mode

---

## Dimension Tables

### DimCustomer
- Customer Name
- Customer ID
- Segment
- Region
- City
- Country
- State

### DimProduct
- Product Name
- Product ID
- Category
- Sub-Category

### DimDate
- Year
- Quarter
- Month
- Weekday
- Season

---

# Data Cleaning & Transformation

Data cleaning was performed using Power Query.

## Cleaning Steps
- Removed duplicates
- Handled null values
- Corrected data types
- Formatted dates
- Renamed columns
- Created calculated columns
- Generated shipping duration metrics

---

# Key DAX Measures

## Total Sales
```DAX
Total Sales = SUM(FactSales[Sales])
```

## Total Profit
```DAX
Total Profit = SUM(FactSales[Profit])
```

## Total Orders
```DAX
Total Orders = DISTINCTCOUNT(FactSales[Order_ID])
```

## Profit Margin %
```DAX
Profit Margin % =
DIVIDE([Total Profit], [Total Sales])
```

## Average Order Value
```DAX
AOV =
DIVIDE([Total Sales], [Total Orders])
```

---

# Dashboard Pages

## 1. Executive Overview Dashboard
Provides a high-level summary of business performance.

### Features
- KPI Cards
- Monthly Sales Trend
- Sales by Region
- Profit by Category
- Top Products Analysis

# Dashboard Screenshot

## Executive Dashboard
<img width="1197" height="675" alt="Screenshot 2026-05-21 183923" src="https://github.com/user-attachments/assets/8835dd36-ff80-4cac-a2e1-09fa14a41e0c" />

---

## 2. Sales Analysis Dashboard

### Features
- Monthly & Quarterly Trends
- Regional Sales Analysis
- Seasonal Revenue Analysis
- Shipping Performance Analysis

  
# Dashboard Screenshot

  ## Sales Dashboard
<img width="1196" height="655" alt="Screenshot 2026-05-23 155935" src="https://github.com/user-attachments/assets/ac398823-394f-4447-8b15-6b62b1ee18ce" />


---

## 3. Product Analysis Dashboard

### Features
- Top Performing Products
- Loss-Making Products
- Category & Sub-Category Analysis
- Product Demand Trends

  # Dashboard Screenshot

  ## Product Dashboard
  <img width="1210" height="680" alt="Screenshot 2026-05-23 155955" src="https://github.com/user-attachments/assets/e822da33-ea28-4a4c-802a-1be9829dc1f9" />


---

## 4. Customer Analysis Dashboard

### Features
- Customer Segmentation
- Top Customers
- Geographic Distribution
- Customer Spending Analysis
- Repeat Customer Insights

  # Dashboard Screenshot
  ## Customer Dashboard
<img width="1187" height="689" alt="Screenshot 2026-05-23 160016" src="https://github.com/user-attachments/assets/922d6e59-ba68-449e-b2d0-abb6c6db45fa" />

---

# Key Business Insights

Some insights derived from the dashboard include:

- Technology category generated the highest revenue
- Certain regions showed low profitability despite strong sales
- High discounts negatively impacted profit margins
- A small percentage of customers contributed a large share of revenue
- Some products consistently generated losses

---

# Project Structure

```bash
Ecommerce-Sales-Analysis/
│
├── Dataset/
├── SQL Queries/
├── Power BI Dashboard/
├── Screenshots/
├── README.md
└── Insights Report/
```

---

# Business Value

This project demonstrates how Business Intelligence tools can help organizations:

- Improve decision-making
- Monitor KPIs effectively
- Identify growth opportunities
- Optimize profitability
- Enhance operational efficiency

---

# Future Improvements

Potential future enhancements include:

- Sales forecasting
- Anomaly detection
- Customer churn prediction
- Inventory optimization
- Real-time dashboard integration

---

# Author

## George

### Connect With Me
- LinkedIn: www.linkedin.com/in/jvtech254
- GitHub: https://github.com/JV-254

---

# Conclusion

This project showcases an end-to-end analytics workflow using Power BI and demonstrates the ability to transform raw business data into actionable insights through interactive dashboards and advanced analytics.
