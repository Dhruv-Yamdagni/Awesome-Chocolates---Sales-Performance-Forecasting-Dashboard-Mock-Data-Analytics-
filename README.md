# Awesome Chocolates - Sales Performance & Forecasting Dashboard

A clean, interactive Power BI business intelligence dashboard built for Awesome Chocolates, a fictional confectionery brand. This project demonstrates star schema dimensional data modeling, sales performance analysis, geographic distribution, and time-series forecasting using synthetic data.

---

## Dashboard Overview

### Page 1: Sales Performance Report
* **Sales Representative Scorecard:** Table displaying sales rep photos, total sales amount, total boxes sold, and amount per box with data bars.
* **Category Breakdown:** Donut and column charts showing revenue distribution across Bars, Bites, and Other products.
* **Geographic Analysis:** Column chart tracking sales performance across India, New Zealand, UK, Canada, USA, and Australia.
* **Team Filter:** Top dropdown slicer to isolate results by sales team.

### Page 2: Sales Trend & Forecasts
* **Customer Acquisition Trends:** Line chart visualizing monthly customer totals with drill-down capabilities.
* **Revenue Forecasting:** Time-series projection utilizing Power BI's forecasting model with a 95% confidence interval through Q1 2022.

---

## Data Model (Star Schema)

* **Fact Table:**
  * `sales` (`Amount`, `Boxes`, `Customers`, `Date`, `Geography`, `Product`, `Sales Person`)
* **Dimension Tables (1-to-many relationships):**
  * `products` (`Category`, `Product`, `Size`)
  * `locations` (`Geo`, `Region`)
  * `people` (`Picture`, `Sales person`, `Team`)

---

## Tech Stack

* Microsoft Power BI Desktop
* DAX (Data Analysis Expressions)
* Star Schema Data Modeling

---

## Getting Started

1. Clone or download this repository.
2. Open `data analysis.pbix` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. Use the slicers, cross-filtering, and visual drill-downs to explore the data.

---

*Note: All data in this repository is synthetic and created strictly for analytical practice and portfolio demonstration.*
