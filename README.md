# Superstore Sales & Profitability Analysis

An exploratory analysis of the Superstore dataset to identify which regions, categories, segments, and discount strategies drive profit — and where the business is losing money.

---

## Question

Which product categories, customer segments, regions, and discount levels drive the most profit for the Superstore, and where are we losing money?

---

## Dataset

- **Source:** Superstore dataset (commonly used retail sample dataset)
- **Size:** ~9,995 rows × 21 columns
- **Time period:** 2014–2017
- **Key fields:**
  - `Sales` – Revenue generated per order
  - `Profit` – Net profit per order
  - `Discount` – Discount applied to the order
  - `Category` – Product category (Technology, Furniture, Office Supplies)
  - `Segment` – Customer segment (Consumer, Corporate, Home Office)
  - `Region` – Geographic region (West, East, Central, South)
  - `Order Date` – Date of transaction

---

## Tools Used

- Microsoft Excel
  - Power Query (for data cleaning & transformation)
  - Pivot Tables
  - Calculated Fields
  - Charts & Visualizations
- Markdown for documentation

---

## Key Findings

1. **Technology is the most profitable category**, generating approximately $145,454.95 in profit and $836,154.03 in sales, outperforming Furniture and Office Supplies in margin performance.

2. **Higher discounts significantly reduce profitability.**  
  Orders with 0–20% discount generated about $421,773.08 in profit, while discounts above 20% resulted in losses of approximately $135,000, showing that larger discounts reduce overall profit.

3. **The Consumer segment drives the highest sales and the highest profit** contributing $1,161,401.34 in revenue, and $134,119.21 in profit

4. **Sales increased from approximately $484,247.50 in 2014 to $733,215.26 in 2017** demonstrating steady revenue growth. 

5. Certain regions generate strong revenue but comparatively weaker profit margins, highlighting operational or pricing inefficiencies.

---

## Visualizations

![Sales and Profit by Region](output/sales-profit-by-region.png)

This chart compares total sales and total profit across regions, highlighting margin differences and regional performance

---

![Sales and Profit by Category](output/sales-profit-by-category.png)

This chart compares total sales and total profit across product categories, highlighting margin differences and category performance.

---

![Discount vs Profit](output/discount-vs-profit.png)

This visualization shows the relationship between discount levels and total profit. Profit declines sharply as discount levels increase, with higher discount bands often resulting in losses.

---

![Monthly Sales & Profit Trend](output/monthly-trend.png)

This trend analysis illustrates revenue growth over time and the volatility of profit across months and years.

---

![Sales and Profit Segment Performance](output/Segment-performance.png)

This chart compares total sales and profit by segment, showing that Consumer leads in revenue while Corporate delivers stronger profit efficiency relative to its sales.

---


## How to Reproduce

1. Clone this repository  
2. Open the dataset from `data/raw/`  
3. Review cleaned data in `data/cleaned/`  
4. Open Excel files or recreate pivot tables using the cleaned dataset  
5. Review detailed findings in `notebooks/analysis-notes.md`

---

## What I'd Do Next

- Analyze profit margins at the sub-category level to identify specific loss-driving products.
- Perform customer-level analysis to evaluate lifetime value and retention patterns.
- Test alternative discount thresholds to determine an optimal pricing strategy.
- Incorporate cost data (if available) to improve margin accuracy.

---
