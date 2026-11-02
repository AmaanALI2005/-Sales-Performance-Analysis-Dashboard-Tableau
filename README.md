Sales Performance Analysis Dashboard | Tableau
An interactive Tableau dashboard built to explore sales performance across markets, months, customers, and products. The project brings together transaction data and supporting customer, date, market, and product tables to present key business metrics in one place.

Project Overview
Objective: Analyze sales performance and make it easier to identify high-performing markets, monthly revenue patterns, and the customers and products contributing most to sales.

Tools: Tableau Public / Tableau Desktop, CSV datasets, Tableau extract (Hyper).
Dashboard Features
- Total Revenue: headline revenue KPI.
- Sales Quantity: headline units-sold KPI.
- Revenue by Market: compares revenue across markets.
- Sales Trend by Month: shows monthly revenue movement.
- Top 5 Customers: highlights the leading customers by the measure used in the workbook.
- Top 5 Products: highlights the leading products by the measure used in the workbook.
- Year and Month Filters: allow users to explore different time periods.
Preview Metrics
The supplied dashboard screenshot displays the following headline values:
KPI	Value shown
Total Revenue	$3.26M
Sales Quantity	4,233


These are values visible in the saved dashboard screenshot, not independently recalculated figures. Results may change when filters or the underlying data are changed.
Repository Structure
 tableau-sales-performance-analysis/
 ├── README.md
 ├── .gitignore
 ├── dashboard/
 │   └── Sales_Performance_Analysis.twbx
 ├── data/
 │   ├── customers.csv
 │   ├── dates.csv
 │   ├── markets.csv
 │   ├── products.csv
 │   └── transactions.csv
 ├── docs/
 │   ├── DATA_DICTIONARY.md
 │   └── PROJECT_NOTES.md
 └── images/
     └── dashboard-preview.png
How to Open the Dashboard
1. Download or clone this repository.
2. Open dashboard/Sales_Performance_Analysis.twbx using Tableau Desktop or Tableau Public (if supported by your installed version).
3. The .twbx is a packaged workbook and includes a Tableau data extract, so it should open without recreating the original local CSV connection.
4. Use the year and month filters to explore the dashboard.
If Tableau asks to locate a data source, connect it to the CSV files in the data/ folder and check the table relationships before refreshing the extract.

Data Model
The project contains five CSV files:
- transactions.csv – transaction-level sales, quantity, date, customer, market, product, and currency fields.
- customers.csv – customer identifiers, names, and customer type.
- dates.csv – calendar attributes such as year and month.
- markets.csv – market names and geographic zones.
- products.csv – product identifiers and product type.
See [Data Dictionary](docs/DATA_DICTIONARY.md) for field descriptions.
Analysis Questions
This dashboard is designed to help answer questions such as:
1. Which markets contribute the most revenue?
2. How does revenue change month by month?
3. Which five customers contribute most to the selected sales measure?
4. Which five products perform best?
5. How do the results change when a year or month is selected?
Important Validation Before Publishing
Please verify the Sales Quantity by Markets worksheet before treating its values as final. In the supplied screenshot, its labels appear as currency amounts and closely match the Revenue by Market values. Confirm that the worksheet uses SUM(sales_qty) rather than SUM(sales_amount), and format the axis and labels as units rather than currency.

Also check whether transaction currencies have been converted to a common currency before aggregating revenue. If INR and USD are both present, do not add them together as if they were the same currency. Document the conversion method if one has been applied.
Skills Demonstrated
- Tableau dashboard development
- KPI reporting and data visualization
- Sales and market performance analysis
- Customer and product performance analysis
- Working with multiple related datasets
- Interactive filtering and business storytelling
Author
Amaan Ali
Aspiring Data Analyst | SQL | Excel | Power BI | Tableau

GitHub: AmaanALI2005
