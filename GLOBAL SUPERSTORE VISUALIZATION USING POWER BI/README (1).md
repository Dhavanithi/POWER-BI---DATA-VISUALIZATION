# Global Superstore Sales & Profit Analysis

## Project Overview

This project analyzes the **Global Superstore dataset** using **Power BI** to understand sales, profit, quantity, discount, shipping cost, customer segments, regions, markets, categories, sub-categories, states, products, and shipping modes.

The project contains:
- A CSV dataset with **1,000 records and 24 columns**
- A Power BI visualization PDF containing multiple charts and matrices
- Business oriented observations and conclusions for every visualization

The main goal is to identify **high-performing categories and regions, profitable customer segments, product-level sales patterns, shipping trends, and the relationship between discount and profit**.

## Dataset Information

### Dataset: Global Superstore

The dataset contains the following major fields:

| Field | Description |
|---|---|
| Row ID | Unique row identifier |
| Order ID | Unique order identifier |
| Order Date | Date on which the order was placed |
| Ship Date | Date on which the order was shipped |
| Ship Mode | Shipping method used |
| Customer ID | Unique customer identifier |
| Customer Name | Customer name |
| Segment | Customer segment |
| City / State / Country | Customer/order location |
| Region | Geographic region |
| Market | Market classification |
| Product ID | Product identifier |
| Category | Product category |
| Sub-Category | Product sub-category |
| Product Name | Product name |
| Sales | Sales amount |
| Quantity | Quantity sold |
| Discount | Discount applied |
| Profit | Profit generated |
| Shipping Cost | Cost of shipping |
| Order Priority | Priority of the order |

### Dataset Summary

- **Records:** 1,000
- **Columns:** 24
- **Total Sales:** 1,710,971.47
- **Total Profit:** 288,920.44
- **Total Quantity Sold:** 5,558
- **Total Shipping Cost:** 272,384.90

## Tools & Technologies

- **Power BI Desktop** – Data visualization and dashboard creation
- **CSV** – Source dataset
- **Data Analysis** – Aggregation and comparison of sales, profit, quantity, discount, and shipping cost

# Visualizations & Conclusions

## 1. Sub-Category Sales and Profit Matrix

This matrix compares **Sales and Profit across product sub-categories**.

### Key Observations
- **Phones** generated the highest sales among the sub-categories, with approximately **417,939.31** in sales.
- Phones also generated the highest profit, approximately **75,119.47**.
- **Appliances, Bookcases, and Copiers** are other strong contributors.
- **Supplies** is the only sub-category showing a negative profit in the dataset.

### Conclusion
**Phones are the strongest sub-category in both sales and profit.** Management should continue supporting high-performing technology products while reviewing low-profit sub-categories such as Supplies.

## 2. Sales by Product Name – Matrix/Bar Visualization

This visualization examines sales at the **individual product level**.

### Key Observations
The highest-selling products in the supplied dataset include:
- Motorola Smart Phone, Full Size
- Apple Smart Phone, Full Size
- Cisco Smart Phone, Full Size
- Nokia Smart Phone, Full Size
- Samsung Smart Phone, Cordless

### Conclusion
**Technology and smartphone-related products have strong product-level sales performance.** Product-level analysis can help identify items that deserve greater inventory availability and marketing attention.

## 3. Quantity and Profit by Sub-Category – Combo Chart

This chart compares **Quantity Sold** and **Profit** for each sub-category.

### Key Observations
- Phones have the highest quantity sold and highest profit.
- Copiers generate strong profit relative to their quantity.
- Appliances and Bookcases also contribute substantially.
- Supplies have low quantity and a negative profit.

### Conclusion
**High sales quantity does not always guarantee the highest profitability.** Businesses should evaluate both volume and profit before deciding which products to prioritize.

## 4. Sales by Region and Market – Stacked Column Chart

This visualization compares sales across regions and markets.

### Key Observations
- **Western Europe** has the highest regional sales in this dataset, approximately **259,576.28**.
- **Oceania** and **Southern Asia** are also major contributors.
- **Asia Pacific** is the largest market by total sales, approximately **800,511.75**.
- USCA has comparatively lower sales in this sample.

### Conclusion
**Asia Pacific is the strongest market, while Western Europe is the strongest individual region.** Expansion and marketing strategies can focus on high-performing markets while investigating opportunities in lower-performing regions.

## 5. Category vs Country – Matrix

This matrix compares sales across **categories and countries/locations**.

### Key Observations
- Technology contributes strongly in several geographic locations.
- Furniture and Office Supplies also contribute to overall sales.
- The visualization helps identify locations where specific categories perform better.

### Conclusion
**Category performance varies by geography.** Regional/category combinations should be considered when planning inventory, promotions, and market-specific strategies.

## 6. Sales and Quantity by Customer Segment – Combo Chart

This chart compares **Sales and Quantity** for Consumer, Corporate, and Home Office segments.

### Key Observations

| Segment | Sales | Quantity | Profit |
|---|---:|---:|---:|
| Consumer | 873,512.42 | 2,741 | 158,231.63 |
| Corporate | 524,287.05 | 1,741 | 88,901.38 |
| Home Office | 313,172.00 | 1,076 | 41,787.43 |

### Conclusion
**Consumer is the strongest customer segment in sales, quantity, and profit.** The Consumer segment should remain a major focus, while Corporate and Home Office segments can be targeted with segment-specific offers.

## 7. Sales by State – Bar Chart

This visualization compares sales across states.

### Key Observations
The leading states in the supplied data include:
- **England:** 83,241.36
- **Queensland:** 60,496.65
- **Ile-de-France:** 53,910.92
- **New South Wales:** 51,867.66
- **Western Australia:** 24,613.23

### Conclusion
**Sales are concentrated in a small number of high-performing states.** These locations can be prioritized for distribution, customer retention, and promotional activities.

## 8. Discount and Profit – Scatter Chart

This scatter chart examines the relationship between **Discount and Profit**.

### Key Observation
The calculated correlation between Discount and Profit in the supplied CSV is approximately **-0.51**, indicating a moderate negative relationship.

### Conclusion
**Higher discounts are generally associated with lower profit in this dataset.** Discount strategies should therefore be carefully controlled so that increased sales volume does not reduce overall profitability.

## 9. Sales by Category and Ship Mode – Stacked Bar Chart

This chart compares sales across **Technology, Furniture, and Office Supplies** for different shipping modes.

### Key Observations
- **Technology** has the highest sales across the categories.
- **Standard Class** contributes the largest sales within each major category.
- Furniture also has strong sales through Standard Class.

### Conclusion
**Standard Class is the most important shipping mode by sales volume, while Technology is the strongest category.** Shipping policies should balance customer delivery expectations with the cost of faster shipping options.

## 10. Shipping Cost by Region and Ship Mode – Stacked Bar Chart

This visualization analyzes **shipping costs across regions and shipping modes**.

### Key Observations
- **Western Europe** has the highest shipping cost in the supplied data, approximately **45,189.14**.
- Oceania and Southern Asia also have relatively high shipping costs.
- Shipping cost varies considerably between regions and shipping modes.

### Conclusion
**Shipping expenses differ significantly across geographic regions.** Optimizing logistics and choosing appropriate shipping modes can help reduce operational costs without negatively affecting customer service.

# Project Objectives

- Analyze sales performance across categories and sub-categories
- Identify the most profitable products
- Compare customer segments
- Analyze regional and market-level sales
- Understand the impact of discounts on profit
- Analyze shipping modes and shipping costs
- Identify high-performing states and regions
- Generate actionable business insights using Power BI

# How to Use This Project

1. Download the `Global_Superstore(CSV).csv` dataset.
2. Open **Power BI Desktop**.
3. Import the CSV file using **Get Data → Text/CSV**.
4. Verify the data types of Sales, Profit, Quantity, Discount, and Shipping Cost.
5. Create the required visualizations using Power BI.
6. Use the provided PDF as the visualization reference.
7. Analyze the charts using the conclusions documented in this README.

# Project Structure

```text
Global-Superstore-Analysis/
│
├── Global_Superstore(CSV).csv
├── Global_Superstore_Visualizationn.pdf
└── README.md
```

