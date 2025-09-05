#  Dynamic Retail Dashboard in Excel  

##  Overview  
The **Dynamic Retail Dashboard** is an interactive and data-driven tool built in Excel to visualize and analyze retail data.  
- Connects to datasets hosted on **GitHub**  
- Uses **Power Query** for data transformation  
- Provides insights via **dynamic charts and KPIs**  
- Solves key business questions, enabling **data-driven decision-making**  

---

##  Datasets Used  

| **Table**      | **Description**                                                                 | **Sample Fields**                                                                                 |  
|-----------------|---------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|  
| **Orders**     | Contains customer order details including product, shipping, and financial data. | Order ID, Returned, Order Date, Ship Date, Ship Mode, Customer Name, Segment, Country, Market, Sales, Profit, Discount |  
| **Returns**    | Tracks orders that have been returned and their associated markets.              | Returned, Order ID, Market                                                                         |  
| **People**     | Information about sales representatives and their regions.                      | Person, Region                                                                                    |  

### 📝 Sample Data  

**Orders Table**  

| Order ID       | Returned | Order Date  | Ship Date   | Ship Mode    | Customer Name | Segment   | Country       | Market | Sales   | Profit  | Discount |  
|----------------|----------|-------------|-------------|--------------|---------------|-----------|---------------|--------|---------|---------|----------|  
| CA-2012-124891 | No       | 31-07-2020  | 31-07-2020  | Same Day     | Rick Hansen   | Consumer  | United States | US     | 2309.65 | 762.18  | 0        |  
| IN-2013-77878  | Yes      | 05-02-2021  | 07-02-2021  | Second Class | Justin Ritter | Corporate | Australia     | APAC   | 3709.40 | -288.77 | 0.1      |  
| IN-2013-71249  | No       | 17-10-2021  | 18-10-2021  | First Class  | Craig Reiter  | Consumer  | Australia     | APAC   | 5175.17 | 919.97  | 0.1      |  

**Returns Table**  

| Returned | Order ID       | Market       |  
|----------|----------------|--------------|  
| Yes      | MX-2013-168137 | LATAM        |  
| No       | US-2011-165316 | LATAM        |  
| Yes      | ES-2013-152578 | EU           |  
| Yes      | CA-2013-118311 | United States|  

**People Table**  

| Person            | Region   |  
|-------------------|----------|  
| Anna Andreadi     | Central  |  
| Chuck Magee       | South    |  
| Kelly Williams    | East     |  
| Matt Collister    | West     |  
| Deborah Brumfield | Africa   |  

---

##  Problem Statements & Solutions  

| **#** | **Analysis**              | **Objective**                                                                 | **Steps**                                                                 | **Visualization**   |  
|-------|----------------------------|-------------------------------------------------------------------------------|----------------------------------------------------------------------------|---------------------|  
| 1     | **KPIs**                  | Calculate Total Sales, Profit, Orders, Quantity & Profit Margin dynamically.   | Import Orders → Create calculated fields → Use Excel formulas → Build KPI table. | KPI Table           |  
| 2     | **Sales & Profit Trends** | Visualize sales & profit trends over time.                                    | Pivot Table (Order Date) → Add Sales & Profit → Line Chart → Apply Slicers. | Line Chart + Slicers|  
| 3     | **Category-Wise Profit**  | Analyze profitability across product categories.                              | Pivot Table (Category vs Profit) → Sort Descending → Add Bar Chart.        | Bar Chart           |  
| 4     | **Segment Sales Share**   | Show contribution of each customer segment.                                   | Pivot Table (Segment vs Sales) → % Share Calculation → Pie/Donut Chart.    | Donut Chart         |  
| 5     | **Sales by Country**      | Compare sales performance across countries.                                   | Pivot Table (Country vs Sales) → Heatmap / Map Chart.                      | Heatmap / Map       |  
| 6     | **Top 5 Subcategories**   | Identify top-performing product subcategories.                                | Pivot Table (Sub-Category vs Sales) → Sort → Filter Top 5 → Column Chart.  | Column Chart        |  
| 7     | **Bottom 5 Subcategories**| Highlight underperforming product subcategories.                              | Pivot Table (Sub-Category vs Sales) → Sort Ascending → Filter Bottom 5.    | Column Chart        |  
| 8     | **Yearly Sales Trends**   | Track sales performance across multiple years.                                | Pivot Table (Yearly Sales) → Line Chart → Slicers for Region/Segment.      | Line Chart          |  

---

##  Dynamic Features  

| **Feature**              | **Description**                                                                 |  
|---------------------------|---------------------------------------------------------------------------------|  
| **Dynamic Charts**        | Updates instantly when slicers/filters are applied.                             |  
| **Power Query Integration** | Automates data cleaning and transformation from raw datasets.                 |  
| **KPI Table**             | Displays critical metrics with icons (💰 for Sales, 📦 for Orders, etc.).        |  
| **Slicers**               | Enables interactive filtering by Category, Market, Country, and Year.           |  

---

##  Next Steps for Extension  

| **Enhancement**        | **Description**                                           |  
|-------------------------|-----------------------------------------------------------|  
| **Return Analysis**    | Investigate return rates by market or category.            |  
| **Customer Insights**  | Identify top & bottom customers based on profitability.    |  
| **Market Analysis**    | Compare performance across different global regions.       |  
| **Product Analysis**   | Evaluate contribution of individual products.              |  

---

##  Significance  
This dashboard enables retail businesses to:  
✔ Track performance using **KPIs**  
✔ Analyze **category, segment, and geographic** trends  
✔ Make **data-driven decisions** to optimize operations  

---

##  Visuals  
The repository includes:  
- Snapshots of the **final dashboard**  
- Visual examples for **each analysis**  

---


