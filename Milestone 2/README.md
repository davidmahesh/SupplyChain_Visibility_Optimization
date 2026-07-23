# Supply Chain Visibility & Inventory Optimization Dashboard

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black">
  <img src="https://img.shields.io/badge/Data%20Analysis-Business%20Intelligence-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Domain-Supply%20Chain-success?style=for-the-badge">
</p>

## Project Overview

Efficient inventory management is one of the most critical factors in supply chain success. Excess inventory increases storage costs, while insufficient inventory leads to stock-outs and customer dissatisfaction.

This project presents an **interactive Power BI dashboard** that transforms raw supply chain data into meaningful business insights. It enables stakeholders to monitor inventory health, evaluate delivery performance, identify slow-moving products, and make data-driven decisions for improving operational efficiency.

The dashboard is designed for:

* Supply Chain Managers
* Inventory Analysts
* Operations Teams
* Business Executives
* Decision Makers

---

# Project Objectives

* Monitor overall inventory performance.
* Calculate and analyze Inventory Turnover Ratio.
* Identify Fast-Moving and Slow-Moving inventory.
* Detect Dead Stock.
* Evaluate order delivery performance.
* Analyze sales trends.
* Improve inventory utilization.
* Reduce operational costs.
* Support strategic business decisions through visual analytics.

---

# Dashboard Features

### Inventory Overview

* Total Inventory Value
* Total Sales
* Inventory Turnover Ratio
* Stock Status Distribution
* Product Category Analysis

### Delivery Performance

* Average Delivery Days
* Late Deliveries
* On-Time Deliveries
* Delivery Performance Trend
* Regional Performance Analysis

### Product Performance

* Fast Moving Products
* Slow Moving Products
* Dead Stock Identification
* Category-wise Inventory Analysis
* Sales Distribution

### Business Insights

* Inventory Efficiency
* Product Demand Analysis
* Revenue Contribution
* Sales Performance
* Operational KPIs

---

# Key Insights

### Inventory

* Products with high turnover contribute significantly to revenue generation.
* Some products remain in inventory for extended periods, increasing holding costs.
* Dead stock occupies valuable warehouse space without generating revenue.

### Delivery

* Late deliveries directly impact customer satisfaction.
* Certain regions experience consistently higher delivery delays.
* Improving logistics planning can reduce transportation inefficiencies.

### Sales

* A limited number of products contribute the majority of sales.
* Category performance varies considerably across the inventory portfolio.
* Inventory optimization presents opportunities to improve profitability.

---

# Business Recommendations

## Inventory Optimization

* Maintain optimal stock levels for high-demand products.
* Reduce excess inventory for low-performing items.
* Perform periodic inventory audits.
* Implement demand forecasting models.
* Improve reorder point calculations.

---

## Supply Chain Improvements

* Monitor supplier performance regularly.
* Reduce transportation delays.
* Optimize warehouse operations.
* Improve inventory replenishment cycles.
* Strengthen logistics coordination.

---

## Sales Strategy

* Promote slow-moving products through targeted campaigns.
* Bundle low-demand items with best-selling products.
* Discontinue consistently underperforming products.
* Focus investment on high-performing categories.

---

# Tools & Technologies

| Technology    | Purpose                        |
| ------------- | ------------------------------ |
| Power BI      | Dashboard Development          |
| Power Query   | Data Cleaning & Transformation |
| DAX           | Business Calculations          |
| Data Modeling | Relationship Management        |
| CSV Dataset   | Source Data                    |
| GitHub        | Version Control                |

---

# Project Workflow

```text
Raw Dataset
      │
      ▼
Power Query (Cleaning)
      │
      ▼
Data Modeling
      │
      ▼
DAX Measures
      │
      ▼
Interactive Dashboard
      │
      ▼
Business Insights
      │
      ▼
Strategic Decision Making
```

---



# Inventory Turnover Calculation Approach

Inventory Turnover Ratio measures how efficiently inventory is sold and replenished during a given period.

### Formula

```text
Inventory Turnover Ratio =
Total Sales
--------------------------
Average Inventory Value
```

### DAX Logic

```DAX
Average Inventory Value =
AVERAGE(Fact_table[inventory_value])

Inventory Turnover Ratio =
DIVIDE([Total Sales],
       [Average Inventory Value],
       0)
```

### Business Interpretation

| Inventory Turnover | Meaning                                         |
| ------------------ | ----------------------------------------------- |
| High Ratio         | Products sell quickly with minimal holding cost |
| Moderate Ratio     | Healthy inventory movement                      |
| Low Ratio          | Excess inventory or weak sales                  |
| Very Low Ratio     | Potential dead stock requiring action           |

A higher turnover ratio generally indicates efficient inventory utilization and stronger cash flow.

---

# Fast-Moving & Slow-Moving Inventory Identification Logic

Inventory movement is determined using the number of days since the last recorded sale for each product.

### Step 1 — Calculate Last Sale Date

```DAX
Last Sale Date =
MAX(Order Date)
```

### Step 2 — Calculate Days Since Last Sale

```DAX
Days Since Last Sale =
DATEDIFF(
    LastSaleDate,
    MaxOrderDate,
    DAY
)
```

### Step 3 — Product Classification

| Days Since Last Sale | Inventory Status |
| -------------------- | ---------------- |
| 0–30 Days            |   Fast Moving    |
| 31–90 Days           |   Normal Moving  |
| 91–180 Days          |   Slow Moving    |
| More than 180 Days   |   Dead Stock     |

### Business Value

This classification helps organizations:

* Reduce warehouse costs
* Improve inventory planning
* Increase product availability
* Eliminate obsolete inventory
* Improve procurement decisions

---

#  Delivery Performance Analysis Methodology

Delivery performance is evaluated by comparing the **actual delivery date** against the **scheduled delivery date**.

### Metrics Used

* Average Delivery Time
* Delivery Delay
* On-Time Delivery Percentage
* Late Delivery Count
* Delivery Performance Trend

### Delivery Classification

| Condition                             | Status           |
| ------------------------------------- | ---------------- |
| Delivered on or before scheduled date | ✅ On Time       |
| Delivered after scheduled date        | ❌ Late Delivery |

### Business Benefits

* Measure logistics efficiency
* Detect shipping bottlenecks
* Improve customer satisfaction
* Optimize transportation planning
* Monitor supplier performance

---

# Key Performance Indicators (KPIs)

*  Total Sales
*  Inventory Value
*  Inventory Turnover Ratio
*  Average Delivery Days
*  Sales Growth
*  Product Performance
*  Category Performance
*  Regional Sales
*  Dead Stock Count
*  Slow Moving Inventory

---


# Dashboard Highlights

* Interactive KPI Cards
* Inventory Health Monitoring
* Delivery Performance Dashboard
* Category-wise Sales Analysis
* Dynamic Filters & Slicers
* Drill-Down Visualizations
* Business-Oriented Insights
* Executive-Level Reporting

---

# Business Impact

This dashboard empowers organizations to:

*  Reduce inventory carrying costs
*  Improve inventory turnover
*  Increase delivery efficiency
*  Maximize profitability
*  Optimize warehouse utilization
*  Support data-driven decision making
*  Enhance supply chain visibility

---

# Author

**David Mahesh Yarlagadda**

**B.Tech – Computer Science & Engineering (AI & ML)**

**Skills:** Power BI • SQL • Python • Data Analytics • Business Intelligence • Machine Learning

---

## If you found this project useful

Please consider giving this repository a **Star ⭐**

It motivates future development and helps others discover the project.

