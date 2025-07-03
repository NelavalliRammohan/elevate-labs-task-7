# Task 7: Basic Sales Summary using SQLite and Python

## Objective
Use SQL inside Python to summarize product sales and display revenue as a chart.

## Tools Used
- Python (sqlite3, pandas, matplotlib)
- SQLite database

## Steps
1. Created `sales_data.db` and `sales` table.
2. Inserted sales data.
3. Queried total quantity and revenue per product using SQL.
4. Loaded results into pandas.
5. Plotted a revenue bar chart.

## SQL Query Used
```sql
SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue
FROM sales
GROUP BY product
