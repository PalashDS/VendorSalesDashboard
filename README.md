# VendorSalesDashboard
Vendor performance Sales Dashboard where I am presenting complete project starting from cleaning the data, storing the data in database using SQL and then data visualization using python and finally Power BI dashboard for General audience to look over and solving business problem.
📊 Vendor Performance Analytics

End-to-End SQL · Python EDA · Statistical Analysis · Power BI Dashboard

This project is a complete Vendor Performance Analysis workflow, taking raw operational data through database design, data engineering, exploratory data analysis, statistical modeling, and interactive dashboard visualization.
It demonstrates how data analysts support business decisions such as vendor optimization, purchasing strategy, brand rationalization, and profit improvement.

🚀 Project Overview

A. The goal of this project is to determine:

1. Which vendors contribute the most to sales & profitability

2. Which brands are top performing vs. underperforming

3. Where the business is losing money (low-margin or negative-profit items)

4. How inventory and purchasing decisions impact profitability

5. Which “hidden gem” brands have low sales but high margins

The workflow integrates SQL, Python, and Power BI to build a scalable and repeatable data insights pipeline.

Data Sources:

purchase_prices.csv
vendor_invoice.csv
purchases.csv
begin_inventory.csv
end_inventory.csv
sales.csv

These files represent purchasing, invoicing, and sales activity for thousands of vendor-brand combinations.

🗄️ 1. Database Design & Data Engineering (SQL)

A SQLite database was created to centralize all vendor-related data.
Using SQL joins, CTEs, and aggregations, a consolidated vendor_sales_summary table was engineered containing:

Total Sales ($)
Total Purchase ($)
Gross Profit & Gross Profit %
Units Sold
Freight Cost
Excise Tax
Stock Turnover
Purchase Contribution %
Unsold Inventory
Sales-to-Purchase Ratio

This forms the analytical backbone for both Python exploration and Power BI reporting.

🧪 2. Exploratory Data Analysis (Python)

Using Pandas, NumPy, Matplotlib, Seaborn, and SciPy, various EDA steps were performed:

✔ Data Cleaning

--> Removed negative or zero profit/margin values
--> Filtered out products with no sales
--> Handled outliers in unit price and margin distributions

✔ Statistical Profiling

--> Identified loss-making SKUs
--> Analyzed vendor-level contribution to revenue
--> Found top-performing and low-performing vendors
--> Segmented “hidden gems” (low sales but high margins)

✔ Statistical Testing (SciPy)

--> Built 95% confidence intervals for vendor profit margins
--> Conducted hypothesis testing to compare top vendors vs. low-performing vendors
--> Verified whether differences in profit margins were statistically significant

📈 3. Power BI Dashboard

A fully interactive Vendor Performance Sales Dashboard was developed, featuring:

🔹 Executive KPIs

Total Sales: $441.41M
Total Purchases: $307.34M
Gross Profit: $134.07M
Avg Profit Margin: 38.72%
Unsold Inventory: 2.71M
Unit Price (Avg): 21.78

🔹 Visual Insights

Purchase Contribution % Donut Chart
Top Vendors by Sales
Top Brands by Sales
Scatter Plot: High vs. Low Performing Vendors

Dynamic drilldowns and filters

📌 Screenshot included in repository.

🔍 Key Insights

* Top 10 vendors contribute ~66% of total purchases (Pareto principle effect).
* Significant margin variation observed between vendors, validated via statistical testing.
* Several brands show high profitability but low sales volume, suggesting marketing/placement opportunities.
* Inventory imbalances and unsold stock highlight procurement inefficiencies.
* Vendor rationalization can reduce cost and improve supply chain stability.

🛠️ Tech Stack
Area	Tools Used
Database	SQLite, SQL (CTEs, Joins, Aggregations)
Data Analysis	Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy
Visualization	Power BI
File Formats	CSV, SQL, PBIX

