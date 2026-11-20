# AdventureWorks Sales Performance Dashboard

## About this project
I used the AdventureWorks database to look at sales performance across products, territories and time. My aim was to turn SQL Server data into a Power BI report that makes the main trends easier to understand and investigate.

## Questions I explored
- How are sales and profit changing over time?
- Which products contribute the most sales?
- How do territories compare?
- Can a user move from the overview to a specific territory?

## Tools
SQL Server, SQL, Power BI Desktop, DAX and Power BI Service.

## What I did
1. Reviewed the AdventureWorks sales data in SQL Server.
2. Prepared a reporting model with a sales fact table and supporting dimension tables.
3. Created measures for total sales, profit, profit margin and year-on-year growth.
4. Built a dashboard with a monthly sales trend, rolling three-month average, top products and territory comparisons.
5. Added a territory drill-through page and tested the `RegionalManager` row-level security role.
6. Published the report to Power BI Service and checked refresh history.

## What I found
- Sales differ substantially across territories, so a company-wide total does not tell the whole story.
- A smaller set of products contributes a large share of sales.
- The monthly chart helps show when sales increase or slow down.
- The territory drill-through makes it easier to investigate individual regions.

**Note:** The 2025 view reflects the transactions available in the dataset and may not represent a complete financial year.

## Dashboard screenshots
![Executive sales dashboard](Screenshots/AW_Executive_Dashboard.jpg)

![Sales data model](Screenshots/AW_Data_Model.jpg)

![Territory drill-through](Screenshots/AW_Territory_Drillthrough.jpg)

![RegionalManager RLS test](Screenshots/AW_RLS_Test.jpg)

Additional evidence is in the `Screenshots` folder, including Power BI Service publication, refresh history, the 2025 filter and the drill-through source.

## Repository folders
- `Data/` – source-data information, where redistribution is permitted
- `SQL/` – saved SQL queries
- `PowerBI/` – Power BI report (`.pbix`)
- `Screenshots/` – dashboard and testing evidence
- `Report/` – completed written report
- `UserGuide/` – instructions for using the dashboard

## How to use the report
Open the `.pbix` file from `PowerBI/` in Power BI Desktop. Use the year selection and dashboard charts to explore results. Right-click a territory in the territory visual to open its drill-through page. The published Power BI Service version may require access to the workspace.

## Limitations and next steps
This is a historical reporting project. It does not include external market factors or sales forecasting. The SQL Server-to-Power BI workflow was implemented; Azure Data Factory was considered as a possible future architecture, not built as part of this solution.

## Author
Franza van den Heever – Data Analytics and Business Intelligence portfolio project.
