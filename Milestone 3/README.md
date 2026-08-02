# Supplier Performance & Transportation Analytics Dashboard

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black">
  <img src="https://img.shields.io/badge/Data%20Analysis-Business%20Intelligence-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Project-Supplier%20Analytics-2E86C1?style=for-the-badge">
</p>

---

# Project Overview

Supplier performance and transportation efficiency are two of the most critical pillars of an effective supply chain. Poor supplier reliability and inefficient transportation routes can increase operational costs, delay customer deliveries, and negatively impact overall business performance.

This project presents an **interactive Power BI dashboard** that evaluates supplier performance, transportation efficiency, carrier effectiveness, and logistics costs using data-driven analytics. The dashboard enables organizations to benchmark suppliers, optimize transportation strategies, and improve supply chain decision-making.

Designed for:

* Supply Chain Managers
* Procurement Teams
* Logistics Managers
* Business Analysts
* Operations Executives

---

# Project Objectives

* Evaluate supplier performance using key business metrics.
* Build a supplier scorecard for performance monitoring.
* Rank suppliers based on operational efficiency.
* Analyze transportation costs across routes and carriers.
* Identify the best-performing logistics partners.
* Monitor delivery consistency and reliability.
* Support strategic sourcing and logistics decisions.
* Reduce operational expenses through data-driven insights.

---

# Dashboard Features

## Supplier Performance

* Supplier Scorecard
* Supplier Ranking
* Quality Performance
* Reliability Analysis
* Lead Time Comparison
* Supplier Benchmarking

## Transportation Analytics

* Transportation Cost Analysis
* Carrier Performance
* Route Performance
* Shipping Cost Distribution
* Delivery Trend Analysis
* Logistics Efficiency

## Business KPIs

* Average Supplier Score
* Average Lead Time
* Supplier Reliability %
* Transportation Cost
* Delivery Performance
* Carrier Efficiency
* Route Utilization

---

# Supplier Scorecard Calculation Methodology

Supplier performance is evaluated using multiple operational KPIs that collectively represent supplier efficiency and reliability.

## Performance Metrics

* Quality Score
* Reliability Percentage
* Average Lead Time
* Delivery Consistency
* Order Fulfillment Performance

## Scorecard Formula

Each supplier receives a composite performance score using weighted business metrics.

```text
Supplier Score =
(Quality Score × 40%)
+
(Reliability × 35%)
+
(Lead Time Score × 25%)
```

Higher scores indicate stronger supplier performance and greater operational reliability.

---

# Supplier Ranking & Benchmarking Approach

Suppliers are benchmarked against one another using their overall performance score.

## Ranking Logic

1. Calculate the supplier score.
2. Sort suppliers in descending order.
3. Assign rankings using DAX.
4. Compare supplier performance against organizational averages.

### Sample DAX

```DAX
Supplier Rank =
RANKX(
    ALL(Dim_Supplier[Supplier Name]),
    [Supplier Score],
    ,
    DESC
)
```

## Benchmark Categories

| Score    | Performance Level    |
| -------- | -------------------- |
| 90–100   | 🟢 Excellent         |
| 80–89    | 🔵 Very Good         |
| 70–79    | 🟡 Good              |
| 60–69    | 🟠 Needs Improvement |
| Below 60 | 🔴 Critical          |

---

# Transportation Cost Analysis Methodology

Transportation costs are analyzed to understand logistics efficiency and identify opportunities for cost optimization.

## Metrics Considered

* Shipping Cost
* Transportation Cost per Order
* Cost by Region
* Cost by Route
* Cost by Carrier
* Average Freight Cost

## Analysis Approach

The dashboard aggregates transportation expenses across different routes, carriers, and geographic regions to identify:

* High-cost transportation lanes
* Expensive carriers
* Cost-effective shipping routes
* Regional logistics variations

This enables organizations to improve logistics planning and reduce unnecessary transportation expenses.

---

# Route & Carrier Performance Evaluation

Transportation efficiency is evaluated by analyzing both routes and logistics carriers.

## Route Evaluation Metrics

* Delivery Success Rate
* Average Delivery Time
* Transportation Cost
* Shipment Volume
* Route Efficiency

## Carrier Evaluation Metrics

* On-Time Delivery %
* Average Transit Time
* Shipping Cost
* Delivery Reliability
* Operational Efficiency

## Performance Classification

| Performance | Status |
| ----------- | ------ |
| Excellent   | 🟢     |
| Good        | 🔵     |
| Average     | 🟡     |
| Poor        | 🔴     |

This evaluation helps businesses identify the most reliable logistics partners while minimizing delivery delays and transportation costs.

---

# Key Performance Indicators

*  Total Suppliers
*  Average Supplier Score
*  Supplier Reliability %
*  Average Lead Time
*  Transportation Cost
*  Route Performance
*  Carrier Performance
*  Delivery Success Rate
*  Logistics Cost Distribution

---

# Key Insights

## Supplier Performance

* Top-ranked suppliers consistently maintain high quality scores and delivery reliability.
* A small group of suppliers contributes to most operational efficiency.
* Some suppliers experience higher lead times, affecting supply chain responsiveness.

## Transportation

* Transportation costs differ significantly across routes and carriers.
* Certain logistics partners consistently achieve higher on-time delivery performance.
* High-cost transportation lanes offer opportunities for optimization.

## Operations

* Benchmarking suppliers helps identify strategic sourcing opportunities.
* Route analysis highlights logistics bottlenecks.
* Carrier comparison enables more informed transportation decisions.

---

# Business Recommendations

## Supplier Management

* Prioritize partnerships with high-performing suppliers.
* Continuously monitor supplier scorecards.
* Conduct regular supplier performance reviews.
* Improve collaboration with medium-performing suppliers.
* Replace consistently underperforming suppliers when necessary.

---

## Transportation Optimization

* Optimize shipping routes to reduce transportation expenses.
* Negotiate pricing with high-cost carriers.
* Increase utilization of reliable logistics partners.
* Monitor transportation KPIs regularly.
* Improve route planning using historical delivery data.

---

## Strategic Business Decisions

* Use supplier benchmarking for procurement planning.
* Build long-term partnerships with top-performing suppliers.
* Implement predictive analytics for supplier risk assessment.
* Improve logistics visibility across the supply chain.
* Support executive decision-making using interactive dashboards.

---

# Tools & Technologies

| Technology    | Purpose                 |
| ------------- | ----------------------- |
| Power BI      | Dashboard Development   |
| Power Query   | Data Transformation     |
| DAX           | Business Calculations   |
| Data Modeling | Relationship Management |
| CSV Dataset   | Source Data             |
| GitHub        | Version Control         |

---

# Project Workflow

```text
Raw Supply Chain Data
          │
          ▼
Data Cleaning (Power Query)
          │
          ▼
Data Modeling
          │
          ▼
DAX Measures & KPIs
          │
          ▼
Supplier Performance Analysis
          │
          ▼
Transportation Analytics
          │
          ▼
Interactive Dashboard
          │
          ▼
Business Insights & Decision Making
```

---

# Dashboard Highlights

* Interactive KPI Cards
* Supplier Scorecards
* Supplier Benchmarking
* Transportation Cost Analysis
* Route Performance Dashboard
* Carrier Comparison
* Dynamic Filters & Drill-Through
* Executive-Level Business Insights

---

# Business Impact

This dashboard helps organizations:

*  Reduce transportation costs
*  Improve supplier selection
*  Benchmark supplier performance
*  Increase logistics efficiency
*  Reduce delivery delays
*  Optimize procurement strategies
*  Improve operational visibility
*  Support data-driven business decisions

---

# Author

**David Mahesh Yarlagadda**
