# Superstore Sales Dashboard — Power BI

An interactive, executive-level sales dashboard built in Power BI Desktop, analyzing sales, profit, orders, quantity, and profitability across categories, sub-categories, and states.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Measures-blue)

## Overview

This dashboard gives a single-page executive summary of Superstore sales performance, with slicers for Year, Category, Payment Mode, State, and Sub-Category. All KPI cards and charts respond dynamically to slicer selections.

## Dashboard preview

| Metric | Value |
|---|---|
| Total Sales | 628K |
| Total Profit | 175K |
| Total Orders | 69 |
| Total Quantity | 1K |
| Profit Margin % | 28% |

## Features

- **Dedicated `_Measures` table** — all DAX measures centralized in one clean, disconnected table for easy maintenance
- **Executive KPI cards** — Total Sales, Total Profit, Total Orders, Total Quantity, Profit Margin %
- **Category performance** — Total Sales by Category, Total Profit by Category, Total Quantity by Category, Total Sales by Sub-Category
- **Regional analysis** — Total Sales by State, Profit Margin % by State
- **Interactive slicers** — Year, Category, Payment Mode, State, Sub-Category
- **Cross-filtering** — selecting any slicer or chart element updates every visual on the page

## Data model

**Source:** `Sales_Dataset.csv`

| Column | Description |
|---|---|
| Order ID | Unique order identifier |
| Amount | Order sales value |
| Profit | Order profit value |
| Quantity | Units sold |
| Category | Product category |
| Sub-Category | Product sub-category |
| PaymentMode | COD, Credit Card, Debit Card, EMI, UPI |
| Order Date | Date of order |
| CustomerName | Customer name |
| State | Customer state |
| City | Customer city |
| Year-Month | Order year-month |

## DAX measures

All measures live in the `_Measures` table.

```DAX
Total Sales = SUM(Sales_Dataset[Amount])

Total Profit = SUM(Sales_Dataset[Profit])

Total Orders = DISTINCTCOUNT(Sales_Dataset[Order ID])

Total Quantity = SUM(Sales_Dataset[Quantity])

Average Sales = DIVIDE([Total Sales], [Total Orders], 0)

Profit Margin % = DIVIDE([Total Profit], [Total Sales], 0)
```

## Dashboard layout

```
┌──────────────────────────────────────────────────┐
│  Title  |  Slicers: Year, Category, PaymentMode,  │
│         |  State, Sub-Category                    │
├──────────────────────────────────────────────────┤
│  Total Sales | Total Profit | Total Orders |      │
│  Total Quantity | Profit Margin %                 │
├──────────────────────────────────────────────────┤
│  Sales by Category | Profit by Category |         │
│  Quantity by Category | Sales by Sub-Category      │
├──────────────────────────────────────────────────┤
│  Sales by State  |  Profit Margin % by State       │
└──────────────────────────────────────────────────┘
```

## How to use

1. Clone or download this repository
2. Open `Superstore_Sales_Dashboard.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
3. If prompted, update the data source path to point to `Sales_Dataset.csv` on your machine
4. Use the slicers at the top to filter by Year, Category, Payment Mode, State, or Sub-Category — all KPI cards and charts update automatically

## Tools used

- Power BI Desktop
- DAX (Data Analysis Expressions)
- Power Query (data load and shaping)

## Repository structure

```
├── Superstore_Sales_Dashboard.pbix   # Power BI dashboard file
├── Sales_Dataset.csv                 # Source dataset
└── README.md                         # This file
```

## Author

Dhavanithi S

## License

This project is for educational and portfolio purposes.
