# Capstone-project
BlinkIT Sales Analysis: SQL-driven data cleaning, KPI calculation, and Power BI visualization to identify sales drivers and optimize outlet performance

###  Project Overview
This project delivers a comprehensive Sales Performance Analysis for the BlinkIT dataset, demonstrating a complete data lifecycle from raw data standardization to interactive visualization.

The core objective was to clean transactional data, derive key performance indicators (KPIs), and identify sales drivers across different product attributes and outlet types. The findings are summarized in a dynamic Power BI dashboard, providing actionable insights into revenue distribution, product profitability, and outlet efficiency.

 ### Technical Stack
 
> Technical Tool Usage
SQL (T-SQL)	Data extraction, cleaning (standardizing fat content), aggregation, advanced calculations (PIVOT, Window Functions).
MS Excel	Initial data inspection and preparation (as implied by the cleaning experience).
Power BI	Data modeling, interactive dashboard design, and visualization of key metrics and trends.


### Key Analytical Insights
The analysis reveals the primary drivers and concentrations of sales across the BlinkIT network:

Product Profitability: Low Fat items are the primary sales driver, generating  approximately 65% of total revenue (776.32K of 1.20M), despite a lower item count than Regular items. Fruits and Vegetables is the leading product category by sales volume.

Outlet Efficiency & Size: The Medium sized outlets are the most productive, contributing the highest proportion of total sales (507.90K). The Supermarket Type 1 outlet overwhelmingly dominates the network's revenue.

Financial Metrics: Total Sales stand at 1.20 Million, supported by 9K items, with a consistent overall Average Rating of 3.92 across the network.

### Data Preparation and SQL Execution

The backbone of this project lies in the robust data preparation and querying performed in SQL.

1. Data Cleaning and Standardization
The Item_Fat_Content column was standardized using a CASE statement to consolidate inconsistent entries (LF, low fat, reg) into two uniform categories: 'Low Fat' and 'Regular', ensuring accurate aggregation.

2. Advanced Analysis and Reporting
Key analytical techniques used to transform the data for reporting include:

### SQL QUERIES
Aggregations & Formatting	Calculated high-level KPIs (Total Sales, Average Sales, Item Count), rounding and casting results to enhance dashboard readability.
PIVOT Function	Transformed item fat content data from rows to columns, enabling direct comparison of Low Fat vs. Regular sales by Outlet Location Type.
Window Functions	Utilized SUM(...) OVER() to calculate the Percentage of Total Sales contributed by different Outlet Size and Outlet Location Type segments.
Segmentation	Created detailed views of sales metrics segmented by Item_Fat_Content, Item_Type, and Outlet_Type.


3. Key Query Example (Percentage of Sales by location)
SQL
<img width="1364" height="513" alt="Screenshot 2025-10-07 221100" src="https://github.com/user-attachments/assets/8ed223c8-df1d-461a-9a3e-9ce00869959a" />


### Interactive Dashboard
<img width="1582" height="847" alt="Screenshot 2025-10-07 204625" src="https://github.com/user-attachments/assets/a794cad8-8b09-4fac-826a-63321f105217" />


The dashboard allows users to dynamically filter sales metrics by Outlet Location Type, Outlet Type, and Outlet Size to explore the data in depth.
