# E-Commerce Sales \& A/B Testing Analysis

An end-to-end data analytics project analyzing 96,000+ orders from the Olist Brazilian E-Commerce dataset using Python, SQL, Excel, and Power BI.

\---

## Project Overview

This project performs a comprehensive analysis of e-commerce sales data covering revenue trends, product performance, customer behaviour, delivery performance, and a statistical A/B test to measure the impact of delivery speed on customer satisfaction.

\---

## Tools \& Technologies

|Tool|Purpose|
|-|-|
|Python (Pandas, NumPy, Matplotlib, Seaborn, Scipy)|Data cleaning, EDA, A/B Testing|
|MySQL|Data storage and business queries|
|Excel|Pivot tables, charts, summary report|
|Power BI|Interactive 4-page dashboard|

\---

## Project Structure

```
ecommerce-analytics/
│
├── data/
│   ├── raw/                  ← Original Olist CSV files
│   └── clean\_orders.csv      ← Cleaned master dataset
│
├── python/
│   ├── 01\_data\_cleaning.ipynb
│   ├── 02\_eda.ipynb
│   └── 03\_ab\_testing.ipynb
│
├── sql/
│   └── analysis.sql
│
├── excel/
│   └── summary\_report.xlsx
│
├── powerbi/
│   └── dashboard.pbix
│
└── README.md
```

\---

## Key Business Insights

|Metric|Value|
|-|-|
|Total Revenue|BRL 19,881,945|
|Total Orders|96,478|
|Total Customers|96,478|
|Avg Order Value|BRL 171.81|
|Avg Review Score|4.09 / 5|
|Late Delivery Rate|6.5%|
|Top Category|Bed, Bath \& Table|
|Top State|São Paulo (SP)|

\---

## A/B Testing — Delivery Speed vs Customer Satisfaction

**Hypothesis:** On-time delivery leads to higher customer review scores.

|Group|Description|Sample Size|Avg Review Score|
|-|-|-|-|
|Group A|On Time / Early Delivery|108,157|4.211|
|Group B|Late Delivery|7,558|2.323|

**Results:**

* Difference in review scores: **1.888 points**
* T-Statistic: **125.79**
* P-Value: **< 0.0001**
* Cohen's d: **1.3176 (Large Effect)**
* Conclusion: **Statistically Significant** — on-time delivery has a large positive impact on customer satisfaction

\---

## Power BI Dashboard

The interactive dashboard covers 4 pages:

1. **Sales Overview** — Revenue KPIs, monthly trend, payment methods
2. **Product Analysis** — Top 10 categories, treemap, category summary
3. **Customer Analysis** — Revenue by state, top states, delivery performance
4. **Delivery \& A/B Test** — A/B test results, delivery performance, key stats

\---

## SQL Analysis

8 business queries covering:

* Monthly revenue trends
* Top 10 product categories by revenue
* Average order value by state
* Repeat vs one-time customer segmentation
* Delivery performance (on-time vs late)
* Payment method breakdown
* Top 10 sellers by revenue
* Review scores by product category

\---

## Dataset

* **Source:** [Olist Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
* **Size:** 100,000+ orders across 8 CSV files
* **Period:** 2016 — 2018

\---

## How to Run

1. Clone this repository
2. Download the dataset from Kaggle and place CSVs in `data/raw/`
3. Run notebooks in order: `01\_data\_cleaning` → `02\_eda` → `03\_ab\_testing`
4. Import `clean\_orders.csv` into MySQL and run `sql/analysis.sql`
5. Open `excel/summary\_report.xlsx` for the Excel report
6. Open `powerbi/dashboard.pbix` in Power BI Desktop

\---

## Author

**Shirley Deepika**
B.E. in Artificial Intelligence \& Data Science
East Point College of Engineering \& Technology, Bengaluru
📧 mshirleydeepika@gmail.com

