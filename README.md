Dynamic Retail Dashboard in Excel
📌 Overview

The Dynamic Retail Dashboard is an interactive and data-driven tool built in Excel to visualize and analyze retail data. It connects to datasets hosted on GitHub, uses Power Query for data transformation, and presents insights through dynamic charts and KPIs. The dashboard solves key business questions, enabling informed decision-making.

📂 Datasets Used
1. Orders Table

Contains details of customer orders, including product, shipping, and financial metrics.

Sample Data

Order ID	Returned	Order Date	Ship Date	Ship Mode	Customer Name	Segment	Country	Market	Sales	Profit	Discount
CA-2012-124891	No	31-07-2020	31-07-2020	Same Day	Rick Hansen	Consumer	United States	US	2309.65	762.18	0
IN-2013-77878	Yes	05-02-2021	07-02-2021	Second Class	Justin Ritter	Corporate	Australia	APAC	3709.40	-288.77	0.1
IN-2013-71249	No	17-10-2021	18-10-2021	First Class	Craig Reiter	Consumer	Australia	APAC	5175.17	919.97	0.1
2. Returns Table

Tracks orders that have been returned, along with the associated markets.

Sample Data

Returned	Order ID	Market
Yes	MX-2013-168137	LATAM
No	US-2011-165316	LATAM
Yes	ES-2013-152578	EU
Yes	CA-2013-118311	United States
3. People Table

Contains details about sales representatives and their respective regions.

Sample Data

Person	Region
Anna Andreadi	Central
Chuck Magee	South
Kelly Williams	East
Matt Collister	West
Deborah Brumfield	Africa
🚀 Problem Statements & Solutions
1. Key Performance Indicators (KPIs)

Objective: Calculate and display Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin dynamically.

Steps:

Import Orders Table into Excel using Power Query.

Create calculated columns:

Profit Margin = Profit / Sales

Total Orders = COUNT(Order ID)

Use Excel formulas:

Total Sales = SUM(Sales)

Total Profit = SUM(Profit)

Total Quantity = SUM(Quantity)

Build a dynamic KPI table with symbols (💰 for Total Sales).

2. Sales and Profit Analysis

Objective: Visualize sales and profit trends over time.

Steps:

Create Pivot Table with Order Date grouped by Year/Month.

Add Sales and Profit as values.

Create Line Chart for trends.

Apply slicers for Category, Market, or Region.

3. Category-Wise Profit

Objective: Analyze profitability across product categories.

Steps:

Pivot Table: Category as rows, Profit as values.

Sort in descending order of Profit.

Use Bar Chart for visualization.

Add slicers for interactivity.

4. Segment-Wise Sales Share (%)

Objective: Show sales proportion for each customer segment.

Steps:

Pivot Table: Segment as rows, Sales as values.

Calculate % Share = Sales / Total Sales * 100.

Use Pie/Donut Chart with labels.

5. Sales by Country

Objective: Analyze sales performance across countries.

Steps:

Pivot Table: Country as rows, Sales as values.

Sort by Sales.

Apply Conditional Formatting or Heatmap.

Optionally, use a Geographic Map Chart.

6. Top 5 Subcategories

Objective: Identify top-performing subcategories.

Steps:

Pivot Table: Sub-Category as rows, Sales as values.

Sort descending.

Filter Top 5.

Column Chart visualization.

7. Bottom 5 Subcategories

Objective: Highlight underperforming subcategories.

Steps:

Pivot Table: Sub-Category as rows, Sales as values.

Sort ascending.

Filter Bottom 5.

Column Chart visualization.

8. Yearly Sales Trends

Objective: Track sales growth across years.

Steps:

Pivot Table: Order Date grouped by Year.

Add Sales as values.

Line Chart visualization.

Add slicers (Category, Region, Segment).

⚡ Dynamic Features

Dynamic Charts → Real-time updates with slicers.

Power Query Integration → Automates data cleaning & transformation.

KPI Table → Highlights critical metrics at a glance.

🔮 Next Steps for Extension

Return Analysis → Investigate return rates by market or category.

Customer Insights → Identify top and bottom customers.

Market Analysis → Compare performance across global regions.

Product Analysis → Deep-dive into product contributions.

🎯 Significance

This dashboard helps retail businesses:

Track performance using KPIs.

Understand category, segment, and geography-based trends.

Make data-driven decisions to improve operations.

🖼 Visuals

This repository includes:

Snapshots of final dashboard.

Visual examples for each problem statement.
