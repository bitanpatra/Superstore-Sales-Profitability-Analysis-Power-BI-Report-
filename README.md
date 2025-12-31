# 📊 Superstore Sales & Profitability Analysis (Power BI Report)

## 1. Business Objective
The objective of this report is to analyze retail sales performance and identify key drivers of profitability.  
The analysis focuses on overall business health, product-level profitability, and the impact of discounting on profit.

This report is designed to support data-driven decision-making related to pricing, product strategy, and regional performance.

---

## 2. Dataset Overview
- **Source:** Sample Superstore dataset  
- **Records:** Retail order-level transactions  
- **Key dimensions:**
  - Date (Order Date, Ship Date)
  - Product (Category, Sub-Category)
  - Geography (Region, State, City)
  - Customer (Segment)
- **Key metrics:**
  - Sales
  - Profit
  - Discount
  - Quantity

---

## 3. Data Preparation & Modeling
The dataset was cleaned and transformed using Power Query in Power BI.

Key preparation steps:
- Corrected date formats using locale-specific parsing (US date format)
- Handled invalid and missing date values without fabricating data
- Created a dedicated Date table to enable time-intelligence analysis
- Derived operational metrics such as shipping duration
- Modeled the data using a star-schema approach with a Date dimension

---

## 4. Key Metrics Defined
The following core metrics were used throughout the report:

- **Total Sales:** Sum of sales revenue  
- **Total Profit:** Sum of profit across transactions  
- **Profit Margin (%):** Total Profit ÷ Total Sales  
- **Average Discount:** Mean discount applied across orders  
- **Trend Metrics:** Quarterly sales and profit trends  

All percentage metrics were calculated at the aggregated level to avoid distortion from row-level calculations.

---

## 5. Report Structure & Analysis

### Page 1: Executive Overview
This page provides a high-level view of overall business performance.

Key analyses include:
- Quarterly sales and profit trends
- Profit contribution by product category
- Regional profitability comparison

This page is intended for rapid assessment of business health and key performance drivers.

---

### Page 2: Product & Discount Analysis
This page focuses on understanding the underlying drivers of profitability.

Key analyses include:
- Relationship between average discount and total profit by sub-category
- Identification of consistently loss-making sub-categories
- Comparison of sales volume versus profitability across products

This analysis highlights how aggressive discounting can negatively impact profit despite strong sales volumes.

---

## 6. Key Insights
- Profitability varies significantly across product categories and sub-categories.
- Certain sub-categories generate high sales but consistently negative profit due to heavy discounting.
- Technology products generally contribute positively to profit, while some Furniture sub-categories underperform.
- Higher discount levels are often associated with lower overall profitability.

---

## 7. Business Recommendations
Based on the analysis:
- Review and limit discounting strategies for low-margin sub-categories.
- Re-evaluate pricing and cost structures for consistently loss-making products.
- Prioritize growth in high-margin categories rather than focusing solely on sales volume.
- Use profitability, not revenue alone, as the primary performance metric.

---

## 8. Tools & Skills Used
- **Power BI** (Data Modeling, DAX, Report Design)
- **Power Query** (Data Cleaning & Transformation)
- **DAX** (Time Intelligence, Profitability Measures)
- **Business Analysis & Data Storytelling**
