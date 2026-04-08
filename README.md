# sales-analytics-dashboard-powerbi
Interactive Power BI dashboard analysing sales performance, customer behaviour, and product trends using DAX and dynamic visualizations.
Sales Analytics Dashboard - Power BI
Project Overview

This project is an interactive Sales Analytics Dashboard built using Power BI. It provides insights into sales performance, customer behavior, and product trends. The dashboard is designed with a focus on usability, performance optimization, and clear data visualization.

Objectives
Analyze overall sales performance
Track total quantity and transactions
Identify top-performing products
Understand customer ratings and payment preferences
Monitor sales trends over time
Key Metrics (DAX Measures)

Total Sales
Total_Sales = 
SUMX('Sales Data', 'Sales Data'[Units Sold] * 'Sales Data'[Price Per Unit])
Total Quantity
Total_Quantity = 
SUM('Sales Data'[Units Sold])
Total Transactions
Total_Transactions = 
COUNTROWS('Sales Data')
Sales Target (5% Growth)
Sales Target = 
[Total_Sales] * 1.05
Dashboard Features
KPI Cards
Total Sales (formatted to 0 decimal places)
Total Quantity
Total Transactions
Average Price
Visualizations
Map showing city-wise sales distribution
Line chart for units sold with drill-down (month to date)
Column chart displaying top 3 mobile models by sales using Top N filter
Pie chart for transaction distribution by payment method
Funnel chart for customer rating analysis
Gauge chart comparing actual sales vs target
Day-wise sales trend analysis
Filters and Interactivity
Month slicer with button-style navigation
Mobile Model filter
Payment Method filter
Brand filter
Day Name filter
Design and Layout
Custom background and branding (logo)
Tile-based layout using a 4-column grid
Consistent styling across visuals using format painter
Clean and structured dashboard for better readability
Key Learnings
Used DAX measures instead of calculated columns to optimize performance
Implemented drill-down functionality for detailed time analysis
Applied Top N filtering for dynamic ranking of products
Improved user experience through structured layout and interactive slicers
Tools and Technologies
Power BI
DAX (Data Analysis Expressions)
Data Visualization
Future Enhancements
Add month-over-month and year-over-year analysis
Implement dynamic tooltips
Integrate larger or real-time datasets
How to Use
Download the .pbix file from this repository
Open it using Power BI Desktop
Use slicers to interact with the dashboard and explore insights
Dashboard Preview
