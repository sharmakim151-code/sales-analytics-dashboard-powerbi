# sales-analytics-dashboard-powerbi
Interactive Power BI dashboard analysing sales performance, customer behaviour, and product trends using DAX and dynamic visualizations.
Sales Analytics Dashboard – Power BI
This project is an end-to-end Sales Analytics Dashboard built using Power BI to track key business metrics like revenue, transactions, customer behavior, and product performance. The dashboard is designed with a strong focus on interactivity, performance optimization, and clean UI/UX.
Project Overview
The dashboard provides insights into:
Total Sales Performance
Quantity Sold & Transactions
Customer Ratings
Payment Method Distribution
City-wise Sales Distribution
Monthly & Daily Sales Trends
Top Performing Products
Key Features & Implementation
UI & Layout Design
Designed a custom background and added branding elements (logo)
Created a tile-based layout (4-column grid) for KPI cards
Used consistent styling across visuals using Format Painter
Built a vertical month slicer panel with button-style navigation
KPI Metrics (DAX Measures)
Total Sales
Total_Sales = 
SUMX('Sales Data', 'Sales Data'[Units Sold] * 'Sales Data'[Price Per Unit])
Formatted to 0 decimal places for better readability
Total Quantity
Total_Quantity = SUM('Sales Data'[Units Sold])
Total Transactions
Total_Transactions = COUNTROWS('Sales Data')
Sales Target (5% Growth)
Sales Target = [Total_Sales] * 1.05
Visualizations
KPI Cards → Total Sales, Quantity, Transactions, Average Price
Map Visualization → City-wise sales distribution
Line Chart → Units sold trend with drill-down (Month → Date)
Column Chart → Top 3 mobile models by sales (Top N filter)
Pie Chart → Transaction distribution by payment method
Funnel Chart → Customer rating breakdown
Gauge Chart → Sales vs Target comparison
Day-wise Sales Trend → Performance across weekdays
Interactive Filters (Slicers)
Month (custom button-style slicer)
Mobile Model
Payment Method
Brand
Day Name
Key Learnings
Optimized performance using measures instead of calculated columns
Implemented Top N filtering for dynamic ranking visuals
Built drill-down hierarchy for detailed time analysis
Enhanced dashboard usability with clean layout and consistent formatting
Dashboard Preview

(Add your screenshot here)
Tools & Technologies
Power BI
DAX (Data Analysis Expressions)
Data Visualization & Dashboard Design
Future Improvements
Add YoY / MoM growth analysis
Implement dynamic tooltips
Integrate real-time or larger datasets
