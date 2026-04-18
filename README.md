# Sales Analytics Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=flat)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

An end-to-end interactive sales analytics dashboard built in Power BI with DAX measures, drill-down analysis, Top N filtering, and 8+ chart types, designed to help business teams monitor performance and make data-driven decisions.

**Live demo:** https://youtu.be/a_GfOACsazM

---

## The business question

How do we give sales teams a single view of performance, by product, region, time, and payment method, without manually updating reports every week?

---

## Key metrics at a glance

| Metric | Value |
|---|---|
| Chart types | 8+ |
| DAX measures | 4 |
| Interactive slicers | 5 |
| Drill-down levels | 2 (month → date) |

---

## Key findings from the data

- Top 3 mobile models account for a disproportionate share of revenue, identified using Top N dynamic filtering
- Sales vs target gap visualised using a gauge chart with a 5% growth target DAX measure
- Drill-down from monthly to daily trend reveals day-of-week patterns invisible in aggregate views

---

## DAX measures

```dax
Total_Sales = SUMX('Sales Data', 'Sales Data'[Units Sold] * 'Sales Data'[Price Per Unit])

Total_Quantity = SUM('Sales Data'[Units Sold])

Total_Transactions = COUNTROWS('Sales Data')

Sales_Target = [Total_Sales] * 1.05
```

---

## Dashboard features

### KPI cards
- Total Sales, Total Quantity, Total Transactions, Average Price
- All built as DAX measures (not calculated columns) for performance optimisation

### Visualisations
- **Map** — city-wise sales distribution
- **Line chart** — units sold with month → date drill-down
- **Column chart** — top 3 products by sales using Top N filter
- **Pie chart** — transactions by payment method
- **Funnel chart** — customer rating analysis
- **Gauge chart** — actual sales vs 5% growth target

### Interactivity
- Month slicer with button-style tile navigation
- Mobile model, payment method, brand, and day name filters
- All visuals cross-filter each other dynamically

---

## What I learned

- **DAX measures over calculated columns** — avoids row-context errors and improves model performance
- **Top N filtering** for dynamic product ranking without hardcoding values
- **Drill-down hierarchy** setup for time-based analysis (month → date)
- **Format painter** to maintain visual consistency across 8+ chart types

---

## Tools used

- Power BI Desktop
- DAX (Data Analysis Expressions)

---

## How to run

1. Download the `.pbix` file from this repo
2. Open in Power BI Desktop (free download from Microsoft)
3. Use the slicers to explore the data interactively

---

## About me

I'm a Data Analyst with 7+ years of experience in EdTech analytics, transitioning into a full-time Data / Business Analyst role. Currently open to opportunities in Bengaluru or remote.

Connect with me on [LinkedIn](https://linkedin.com/in/diksha-sharma-ab2081127)
