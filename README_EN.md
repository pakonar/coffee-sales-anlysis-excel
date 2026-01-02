# Sales & Profitability Dashboard – Coffee Roast Co.

![Dashboard Coffee Roast Co - Liberica Analysis](dashboard.png)

## 1. Project Objective
The objective of this project was to develop an interactive operational report for **"Coffee Roast Co."**, a coffee distributor. The dashboard is designed to monitor Key Performance Indicators (KPIs) and support commercial decision-making across the USA, UK, and Ireland markets, based on historical data from 2019–2022.

## 2. Data Source & Structure
The data used in this project is sourced from the open repository: [excel-project-coffee-sales](https://github.com/mochen862/excel-project-coffee-sales).
The analysis is based on three Excel worksheets:
* **Orders:** Transaction log (Order IDs, dates, quantities).
* **Customers:** Customer demographics, locations, and loyalty status.
* **Products:** Pricing, unit costs, and coffee roast/type specifications.

## 3. Business Questions
The report was designed to answer the following questions:
* **Sales Trends:** How has revenue evolved over time, and which countries dominate sales?
* **Product Mix Analysis:** Which coffee types (Arabica, Robusta, Liberica, Excelsa) are the most profitable?
* **Loyalty Effectiveness:** What is the contribution of loyalty card members to the overall results?
* **Customer Concentration:** How dependent is the company on its top 5 customers?

## 4. Tools & Techniques
* **Excel – Data Preparation (ETL):** Connected data from three sheets using **XLOOKUP** and **INDEX/MATCH**. Performed data cleaning and created custom calculated columns to determine net profit per order.
* **Excel – Analysis:** Utilized Pivot Tables for data aggregation and Calculated Fields for profit margin percentages.
* **Advanced Interactivity:** Implementation of **static baselines** – Total Revenue and Total Profit indicators were intentionally disconnected from slicers to allow for a constant comparison of a selected segment’s performance against the company’s total scale.
* **Dashboard Design:** Integrated **Timelines** and **Slicers** for dynamic filtering by: time, coffee type, roast type, package size, and loyalty status.

## 5. Key Performance Indicators (KPIs)
The dashboard employs a system of dynamic KPI cards showing absolute values and their percentage share of the total business:
* **Total Revenue & Total Profit:** Static baselines representing the company's overall scale of operations.
* **Segment Revenue (% of Total Revenue):** The selected segment's share of total revenue.
* **Segment Profit (% of Total Profit):** A key indicator of a segment's profitability relative to the entire company.
* **Segment Orders (% of Total Orders):** The segment's share of total order volume.

---

## 6. Key Insights

### Sales Trends & Geographical Analysis
Revenue showed steady growth from $12.2k (2019-2020) to $13.8k in 2021 (approx. **13% increase**). 2022 data indicates a slowdown in momentum.
* **US Dominance:** The US market share is growing consistently – from 78% in 2019 to a record **82%** in 2022.
* **Risk:** The company is becoming heavily financially dependent on a single market.
* **Recommendation:** Marketing efforts should be intensified in European markets to diversify revenue streams and mitigate geographical risk.

### Product Mix & Profitability (Segment Share)
Using static baselines revealed significant performance disparities:
* **High Profitability of Liberica:** Accounting for 25% of order volume, it generates **35% of total profit** ($1.57k). This is the highest-margin product.
* **Low Efficiency of Robusta:** Despite its popularity (24% of orders), its real impact on total profit is only **12%** ($0.54k).
* **Conclusion:** Optimization efforts should focus on promoting Liberica rather than chasing volume in the low-margin Robusta segment.

### Loyalty Program Effectiveness
* **Sales Foundation:** Loyalty card members account for nearly half of the company's performance (**48% of orders and 46% of profit**).
* **2021 Shift:** During the company's record year, there was a sudden spike in orders from non-loyalty customers.
* **Next Steps:** An analysis of unique Customer IDs is required to determine if this growth came from new customer acquisition or existing customers opting out of the loyalty program.

### Customer Concentration
* **Stability:** The top 5 largest customers combined generate only **5.85% of total revenue** (the largest single customer accounts for 1.31%).
* **Conclusion:** This low concentration indicates a perfectly diversified customer base. The business is resilient against the loss of any single client, ensuring high financial stability.
