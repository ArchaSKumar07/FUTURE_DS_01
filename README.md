# FUTURE_DS_01
🛒 Superstore Sales Dashboard (Power BI)
An interactive Power BI dashboard for exploring Superstore sales performance across different dimensions such as time, region, category, and customer segments. This tool is useful for business analysts, data enthusiasts, and managers to gain actionable insights into operational and sales efficiency.
📌 Table of Contents
Features

Dataset Details

Dashboard Overview

Key Metrics (DAX)

Project Goals

Getting Started

Folder Structure

Screenshots

Contributing

License

📊 Features
KPI Cards:

Total Quantity Sold

Total Sales (formatted as ₹K)

Number of Returns

Total Profit

Time Series Analysis:

Monthly Sales Trend

Year-over-Year Sales Growth

Monthly Profit Tracking

Product Analytics:

Sales by Category (Furniture, Technology, Office Supplies)

Sales by Subcategory (Phones, Binders, Chairs, etc.)

Customer Segmentation:

Pie chart of sales by segment: Consumer, Corporate, Home Office

Shipping & Payment Insights:

Sales by Ship Mode (Standard, Second Class, Same Day)

Sales by Payment Mode (Credit Card, Cash, etc.)

Geographic Performance:

Map of sales and profit by US states

Interactive Filters:

Region (West, East, Central, South)

Time period

Category and Segment

📁 Dataset Details
You can use the classic Superstore dataset (available on Kaggle, Tableau, etc.) or your own:

Tables Used:

Orders: Order ID, Order Date, Customer Name, Segment, State, Region

Order_Details: Order ID, Product Name, Category, Subcategory, Sales, Profit, Quantity, Discount

Returns: Optional — shows returned orders for analysis

Targets: Optional — used to compare actual performance vs. targets

🧠 Key Metrics (DAX)
Some of the DAX measures used:

DAX
Copy
Edit
Total Sales = SUM(Order_Details[Sales])

Total Profit = SUM(Order_Details[Profit])

Total Quantity = SUM(Order_Details[Quantity])

Total Returns = COUNT(Returns[Order ID])

Sales by Year = CALCULATE([Total Sales], YEAR(Orders[Order Date]))

Monthly Profit = CALCULATE([Total Profit], DATESMTD('Date'[Date]))
Time intelligence, filters, and slicers enhance this analysis further.

🎯 Project Goals
Clean, transform, and model e-commerce sales data

Track key performance indicators (KPIs)

Detect profitable categories and underperforming segments

Provide region-wise insights to improve logistics and marketing

Understand customer behavior through segment and category breakdowns

