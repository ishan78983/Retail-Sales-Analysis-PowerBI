# Retail Sales Analysis (Power BI)

## Overview
This project presents an interactive Power BI dashboard analyzing retail sales data to uncover key business insights.  
The dashboard provides an overview of sales performance, customer behavior, and product category trends.  
Data was cleaned and transformed using Power Query, and DAX measures were created for KPIs and advanced analysis.

## Project Highlights
- **KPIs:** Total Sales, Total Orders, Average Order Value, Profit %  
- **Trends:** Monthly sales trend, peak sales months  
- **Customer Insights:** Customer demographics and purchasing patterns  
- **Category Analysis:** Top-performing product categories and sub-categories  
- **Interactivity:** Filters and slicers for region, category, and time  

## Project Files
- `Retail_Sales_Dashboard.pbix` — Power BI dashboard file  
- `data/retail_sales.csv` — Source dataset  
  

## Data & Modeling
- **Source:** Retail sales dataset (CSV format)  
- **Transformations:** Data type corrections, handling null values, and creating a proper date column  
- **Modeling:** Star schema with fact table and dimension tables  
- **Measures (DAX):**  
```DAX
Total Sales = SUM(Retail_sales[total_sale])

Total Orders = COUNT(Retail_sales[transactions_id])

Avg Order Value = DIVIDE([Total Sales], [Total Orders], 0)

Profit = SUM(Retail_sales[total_sale]) - SUM(Retail_sales[cogs])

Profit % = DIVIDE([Profit], [Total Sales], 0)
# Retail Sales Analysis (Power BI)

## Overview
This project presents an interactive Power BI dashboard analyzing retail sales data to uncover key business insights.  
The dashboard provides an overview of sales performance, customer behavior, and product category trends.  
Data was cleaned and transformed using Power Query, and DAX measures were created for KPIs and advanced analysis.

## Project Highlights
- **KPIs:** Total Sales, Total Orders, Average Order Value, Profit %  
- **Trends:** Monthly sales trend, peak sales months  
- **Customer Insights:** Customer demographics and purchasing patterns  
- **Category Analysis:** Top-performing product categories and sub-categories  
- **Interactivity:** Filters and slicers for region, category, and time  

## Project Files
- `Retail_Sales_Dashboard.pbix` — Power BI dashboard file  
- `data/retail_sales.csv` — Source dataset  
- `screenshots/` — Dashboard preview images  

## Dashboard Preview
### Overview
![Dashboard Overview](screenshots/overview.png)

### Sales Trend
![Sales Trend](screenshots/sales_trends.png)

### Category Performance
![Category Performance](screenshots/category_performance.png)

## Data & Modeling
- **Source:** Retail sales dataset (CSV format)  
- **Transformations:** Data type corrections, handling null values, and creating a proper date column  
- **Modeling:** Star schema with fact table and dimension tables  
- **Measures (DAX):**

```DAX
Total Sales = SUM(Retail_sales[total_sale])

Total Orders = COUNT(Retail_sales[transactions_id])

Avg Order Value = DIVIDE([Total Sales], [Total Orders], 0)

Profit = SUM(Retail_sales[total_sale]) - SUM(Retail_sales[cogs])

Profit % = DIVIDE([Profit], [Total Sales], 0)
```




### How to Use

Download the Power BI file .pbix.

Open in Power BI Desktop.

If required, update the dataset path:

Go to Transform data → Data source settings → Change Source.

Refresh the data using Home → Refresh.


#Conclusion

This Power BI dashboard serves as a data analysis project for retail sales, providing actionable insights into customer behavior, sales performance, and category trends. It demonstrates skills in Power Query, DAX, and dashboard design.
