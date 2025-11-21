# 🚀 Sales Performance & Profitability Analysis Dashboard

## 🌟 Project Overview and Goal

This Power BI solution was developed to deliver a comprehensive, interactive view of retail sales performance, focusing on identifying growth drivers and areas where profit margins were being eroded. The analysis covers full transaction history across *three fiscal years (2022–2024)*.

* *Objective:* To move beyond basic reporting and provide executive-level insights for optimizing regional sales strategies and managing product portfolio profitability.
* *Key Finding Summary:* The dashboard successfully pinpointed a significant seasonal drop in margin performance, allowing the leadership team to implement targeted inventory adjustments for the next cycle.

---

## 🛠 Tools and Technologies Used

| Tool/Technology | Purpose and Application |
| :--- | :--- |
| *Power BI Desktop* | Visualization, Data Modeling, and Dashboard Design. |
| *Power Query (M Language)* | Advanced ETL (Extract, Transform, Load) processes, including conditional column creation and data pivoting. |
| *DAX* | Creation of complex time-intelligence functions (DATEADD, CALCULATE) and custom KPIs (e.g., Churn Rate). |
| *Data Source* | Raw Retail Transactional Data (approx. 500,000 rows). |

---

## ⚙ Analysis Methodology (Deep Dive)

### 1. Data Preparation and Cleaning
* *Source Data:* Received raw data from four separate Excel files requiring consolidation.
* *Key Transformations:* Used Power Query to *unpivot* product categories for effective filtering, corrected inconsistent date formats, and implemented conditional logic to standardize regional naming conventions. *Missing values in the 'Discount' column were handled by imputing the median value.*

### 2. Data Modeling and DAX Calculations
* *Model Structure:* A robust Star Schema model was implemented, defining one central Fact table (Sales) linked to Dimension tables (Date, Product, Region) for optimized query performance.
* *Custom Measures:* Crucial KPIs were calculated using DAX to enable advanced analysis:
    * *YoY Growth:* Measures year-over-year revenue expansion.
    * *Margin Erosion:* Calculated as Profit Margin % (Current Period) vs. Profit Margin % (Previous Period).
    * *RankX:* Used to dynamically rank top-performing products/regions.

### 3. Visualization and Design
* *Design Philosophy:* Followed the "Information Density" principle, ensuring all key metrics are visible without clutter.
* *Interactivity:* Implemented drill-through filters allowing users to move from the high-level summary to detailed transaction data.
* *Visual Elements:* Strategic use of trend lines, heat maps, and gauge visuals to provide instant status checks on profitability targets.

---

## 💡 Key Insights and Business Findings

The analysis successfully delivered the following critical business insights:

* *Profitability:* Total Gross Profit for the period was *$1.2 Million* on *$8.5 Million* in total revenue.
* *Growth:* Achieved *15% Year-over-Year* revenue growth, primarily driven by the "Smart Accessories" product category.
* *Regional Disparity:* The *'East' region* showed a consistent *35% underperformance* in profit margin compared to the national average, suggesting a need for targeted marketing or pricing review in that specific area.
* *Seasonal Trends:* Identified a critical drop in customer acquisition rate during the December holiday season, contrary to expectations.

