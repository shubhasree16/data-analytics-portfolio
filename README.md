# data-analytics-portfolio
Adventure Works datasets
📊 Sales Executive Cockpit – Dynamic Dashboard
1. 🧭 Background and Overview
Sales leaders in modern organizations need real-time, actionable insights to monitor sales performance, identify bottlenecks, and optimize team efforts across territories. This project simulates the development of a Sales Executive Cockpit Dashboard using the AdventureWorks dataset—a mock B2B manufacturing and distribution business.

The goal is to empower leadership with a single view of performance KPIs, with drill-down capabilities by region, product line, and sales representatives.

🔧 Tools Used: SQL Server | Power BI | Excel | DAX | Python (for optional forecasting)

2. 🗂️ Data Structure Overview
This use case draws data from several interlinked AdventureWorks tables:

Table	Description
Sales.SalesOrderHeader	One row per sales order, includes order date, customer ID, sales person ID, territory ID, total due
Sales.SalesOrderDetail	Line-item detail for each order: product ID, quantity, unit price
Sales.Customer	Customer info with links to geography and store
Sales.SalesTerritory	Regional sales zones with country/group-level segmentation
Sales.SalesPerson	Contains each salesperson’s data: quotas, bonus, commission, sales YTD
Production.Product	Product-level info like name, subcategory, list price, cost
Production.ProductCategory / ProductSubcategory	Product hierarchy for slicing and grouping
Person.Person	Names and contact info for sales staff

Relationships built using SalesOrderHeader.SalesPersonID, Customer.CustomerID, SalesOrderDetail.ProductID, and SalesOrderHeader.TerritoryID.

3. 🧑‍💼 Executive Summary
The Sales Executive Cockpit enables a leadership team to monitor:

📈 Total Sales Revenue & YoY Growth

🏆 Top Performing Sales Reps and Territories

📦 Best-Selling Product Categories

🧮 Average Order Value (AOV) and Sales per Rep

🎯 Quota Achievement by Salesperson

Key findings from this dashboard highlight regional disparities in performance, underperforming product lines, and quota gaps among certain team members.

4. 🔍 Insights Deep Dive
A. Sales Performance Trends

Monthly trend analysis reveals Q4 spike in sales across all regions, likely tied to year-end purchasing cycles.

YoY comparison shows a 12.4% increase in revenue, primarily driven by North America.

B. Top Territories

North America and Europe dominate in both volume and revenue.

APAC territories have strong average order values but fewer transactions—suggesting high-value but infrequent buyers.

C. Salesperson Leaderboard

Top 3 reps contribute over 45% of total sales.

20% of sales reps did not meet 75% of their sales quotas—opportunity for reallocation or training.

D. Product Performance

Accessories category shows highest volume but lowest margin.

Bikes category leads in revenue but has high variance in unit sales, indicating pricing or availability issues.

E. Customer Insights

Top 10% of customers account for 60% of revenue—Pareto pattern confirmed.

Repeat customers tend to order within 60–90 day cycles—potential to introduce upsell campaigns mid-cycle.

5. ✅ Recommendations
Reallocate Sales Quotas based on historic territory performance to align incentives with regional potential.

Coach Underperforming Reps using leaderboard insights and benchmark metrics.

Introduce Bundle Promotions for low-margin products in Accessories to boost AOV.

Double Down on Repeat Customer Strategy—set automated reminders for sales reps around the 60–90 day re-purchase window.

Enable Dynamic Territory Monitoring—add filters by country group to ensure agile response to regional performance shifts.

