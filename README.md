# 📊 Amazon Customer & Sales Analytics Dashboard (Power BI)

## 📊 Project Overview
This end-to-end **Power BI solution** analyzes customer behavior, regional sales performance, and loyalty trends for Amazon retail data.  

The goal was to transform raw transactional data into a **strategic decision-making tool** that identifies high-value customers and operational bottlenecks.


## 🖼️ Dashboard Preview

| Page |                       Key Features |
|-----------------------|-----------------------------------------------------------|
| **Executive Summary** | High-level KPIs: Revenue, AOV, and Satisfaction scores |
| **Customer Insights** | Spend vs Frequency mapping and retention analysis |
| **Regional Performance** | Geographic distribution of sales and fulfillment status |
| **Drill-through Detail** | Granular row-level analysis for state-wise insights |

## 💡 Business Value

This dashboard answers critical **"So What?"** questions for management:

- **Who are our VIPs?**  
  Identifies customers with high spend and high order frequency.

- **Where is the friction?**  
  Tracks delivery status and satisfaction scores across categories.

- **What drives growth?**  
  Compares YoY performance across different membership types (Annual vs Monthly).
## 🛠️ Technical Deep-Dive

### 1. Data Architecture (Star Schema)
The model is built on a **Star Schema** for performance and scalability:

- **Fact Table:** Amazon (sales and customer transactions)
- **Dimension Tables:**
  - DimDate (Time intelligence)
  - UserAccess (RLS & Geography)
- **Measures Table:** Dedicated DAX table containing all business logic

### 2. Advanced DAX Implementation
Key measures include:

- **AOV YoY %**
  - Year-over-year growth with dynamic conditional formatting (arrows)

- **Churn Probability**
  - Logic-based categorization of customer risk

- **Days Parameter (What-If Analysis)**
  - Allows dynamic adjustment of analysis window

### 3. UX Features (Drill-through & Tooltips)

- **Drill-through**
  - Right-click any state or category to access “Customer Details” page

- **Report Page Tooltips**
  - Hover-based deep-dive insights without leaving the main view
