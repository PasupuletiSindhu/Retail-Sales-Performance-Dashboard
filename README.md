# Retail Sales Performance Dashboard – Power BI

This project analyzes regional, product-level, and time-based sales performance using **Power BI**. It provides a comprehensive and interactive view into key performance indicators (KPIs) to support business decisions in retail management.

## Dashboard Preview
Please check DashBoard.png for the preview

## Project Objective
Design a business-ready dashboard that enables decision‑makers to:
- Monitor total sales, profits, and profit margins
- Identify top‑performing regions, segments, and products
- Analyze trends over time (monthly and quarterly)
- Optimize pricing, discounts, and inventory strategy

## Dataset
- **Source:** Kaggle – Superstore Dataset  
  <https://www.kaggle.com/datasets/vivek468/superstore-dataset-final>
- **Data File:** `SampleSuperstore.csv`
- **Content:** Retail order data including sales, profit, quantity, category, sub‑category, region, customer segment, discount, and dates

## Tools & Technologies
- Power BI Desktop
- DAX (Data Analysis Expressions)
- Power Query (M Language)
- Data Modeling
- Interactive Slicers and Filters

## Features & Methods

### Data Cleaning & Transformation
- Fixed data types, handled missing values, and removed duplicates
- Extracted `Year`, `Month`, and `Quarter` from `Order Date`
- Calculated `Profit Margin` as a custom column

### DAX Measures
```DAX
Total Sales      = SUM(SalesData[Sales])
Total Profit     = SUM(SalesData[Profit])
Profit Margin %  = DIVIDE([Total Profit], [Total Sales])
Average Discount = AVERAGE(SalesData[Discount])
```

### Visuals Included
- **KPI Cards:** Total Sales, Total Profit, Profit Margin, Quantity
- **Bar Chart:** Sales by Region (sorted high to low)
- **Donut Chart:** Sales by Category
- **Line Chart:** Monthly Sales Trend
- **Bar Chart:** Top 10 Products by Sales
- **Column Chart:** Profit Margin by Segment
- **Slicers:** Region, Segment, Category, Year

## Key Business Insights
- Central region leads in revenue but shows a lower profit margin because of heavy discounting.
- Technology category has the highest year‑over‑year sales growth yet thinner margins.
- Top 10 products contribute roughly 45 percent of total revenue, highlighting areas for inventory focus.
- Corporate segment delivers the highest average profit margin compared with Consumer and Home‑Office segments.

## Dashboard Access
Add your Power BI Service published link here, or include the `.pbix` file in this repository for local exploration.

## How to Use
1. Clone or download this repository.
2. Open `Retail Sales Performance Dashboard.pbix` in Power BI Desktop.
3. Refresh the data (optional) and interact with slicers for different perspectives.


## License
This project is provided for educational use. Feel free to share or adapt with appropriate credit.
