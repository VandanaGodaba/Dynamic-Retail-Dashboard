Sure! Here's an updated and extended version of the **README** with **sample tables** included for the "Orders," "Returns," and "People" tables. The sample data will help users understand the structure of your dataset and how it's used in the dashboard.

---

# Dynamic Retail Dashboard in Excel

## Overview

The **Dynamic Retail Dashboard** is an Excel-based business intelligence tool designed to help retail professionals analyze their business performance effectively. This dashboard integrates data from multiple sources and provides actionable insights through interactive visualizations and dynamic reporting.

The project uses three primary tables (Orders, People, and Returns) that are connected to the Excel file hosted on GitHub. The data is processed using **Power Query** to perform essential transformations, and the dashboard leverages **PivotTables**, **dynamic charts**, and **key performance indicators (KPIs)** to allow for real-time analysis.

This dashboard helps retail businesses track important metrics, analyze sales performance, and identify trends, providing insights that can drive business decisions.

---

## Table of Contents

- [Overview](#overview)
- [Tables Used](#tables-used)
  - [Orders Table](#orders-table)
  - [Return Table](#return-table)
  - [People Table](#people-table)
- [Key Metrics (KPIs)](#key-metrics-kpis)
- [Problem Statements Solved](#problem-statements-solved)
- [Dashboard Features](#dashboard-features)
- [Steps to Create the Dashboard](#steps-to-create-the-dashboard)
- [Future Steps](#future-steps)
- [Data Dictionary](#data-dictionary)
- [Adding Visuals](#adding-visuals)

---

## Tables Used

The dashboard integrates data from the following tables, each representing a key aspect of retail operations. These tables are hosted on GitHub and connected to the Excel file using **Power Query**.

### 1. **Orders Table**
Contains detailed information about each customer order, including shipping details, product categories, sales, and profit.

**Sample Data for Orders Table:**

| Row ID | Order ID           | Order Date | Ship Date  | Ship Mode    | Customer ID | Customer Name  | Segment  | City         | State   | Country     | Postal Code | Market | Region | Product ID         | Category   | Sub-Category | Product Name                                      | Sales   | Quantity | Discount | Profit  | Shipping Cost | Order Priority |
|--------|--------------------|------------|------------|--------------|-------------|-----------------|----------|--------------|---------|-------------|-------------|--------|--------|--------------------|------------|--------------|--------------------------------------------------|---------|----------|----------|--------|---------------|----------------|
| 32298  | CA-2012-124891     | 31-07-2020 | 31-07-2020 | Same Day     | RH-19495    | Rick Hansen     | Consumer | New York City| New York| United States| 10024       | US     | East   | TEC-AC-10003033     | Technology | Accessories   | Plantronics CS510 - Wireless Headset            | 2309.65 | 7        | 0        | 762.18 | 933.57        | Critical       |
| 26341  | IN-2013-77878      | 05-02-2021 | 07-02-2021 | Second Class | JR-16210    | Justin Ritter   | Corporate| Wollongong   | NSW     | Australia   | -           | APAC   | Oceania| FUR-CH-10003950     | Furniture  | Chairs        | Novimex Executive Leather Armchair, Black       | 3709.40 | 9        | 0.1      | -288.77| 923.63        | Critical       |
| 25330  | IN-2013-71249      | 17-10-2021 | 18-10-2021 | First Class  | CR-12730    | Craig Reiter    | Consumer | Brisbane     | Queensland| Australia  | -           | APAC   | Oceania| TEC-PH-10004664     | Technology | Phones        | Nokia Smart Phone, with Caller ID               | 5175.17 | 9        | 0.1      | 919.97 | 915.49        | Medium         |
| 13524  | ES-2013-1579342    | 28-01-2021 | 30-01-2021 | First Class  | KM-16375    | Katherine Murray| Home Office| Berlin      | Berlin  | Germany     | -           | EU     | Central| TEC-PH-10004583     | Technology | Phones        | Motorola Smart Phone, Cordless                 | 2892.51 | 5        | 0.1      | -96.54 | 910.16        | Medium         |

---

### 2. **Return Table**
Contains data on product returns, including the order ID and market where the return occurred.

**Sample Data for Return Table:**

| Returned | Order ID          | Market  |
|----------|-------------------|---------|
| Yes      | MX-2013-168137    | LATAM   |
| Yes      | US-2011-165316    | LATAM   |
| Yes      | ES-2013-1525878   | EU      |
| Yes      | CA-2013-118311    | United States |
| Yes      | ES-2011-1276768   | EU      |
| Yes      | MX-2013-131247    | LATAM   |
| Yes      | ID-2011-20975     | APAC    |
| Yes      | IN-2014-58460     | APAC    |
| Yes      | ES-2011-3028321   | EU      |

---

### 3. **People Table**
Contains information about employees or key personnel and their corresponding regions.

**Sample Data for People Table:**

| Person           | Region         |
|------------------|----------------|
| Anna Andreadi    | Central        |
| Chuck Magee      | South          |
| Kelly Williams   | East           |
| Matt Collister   | West           |
| Deborah Brumfield| Africa         |
| Larry Hughes     | AMEA           |
| Nicole Hansen    | Canada         |
| Giulietta Dortch | Caribbean      |
| Nora Preis       | Central Asia   |

---

## Key Metrics (KPIs)

The dashboard tracks several key performance indicators (KPIs), which provide a quick overview of the business performance. These KPIs are dynamically updated based on the selected filters and data inputs.

| KPI Name        | Symbol | Description                                                   |
|-----------------|--------|---------------------------------------------------------------|
| **Total Sales**     | 💰     | Sum of all sales revenue from all orders.                     |
| **Total Profit**    | 📈     | Sum of profits generated from all orders.                     |
| **Total Quantity**  | 📦     | Total number of items sold across all orders.                 |
| **Total Orders**    | 🛒     | Total number of orders placed by customers.                   |
| **Profit Margin**   | 💹     | Average profit margin for all orders (Profit/Sales).          |

These KPIs are displayed dynamically on the dashboard and are automatically updated when new data is loaded.

---

## Problem Statements Solved

The **Dynamic Retail Dashboard** addresses several business problems and provides insights that can guide strategic decisions. Below are the problem statements solved by this dashboard:

### 1. **Total Sales, Profit, Quantity, and Number of Orders**

- **Insight**: Understand the overall performance of the business by tracking total sales, profit, quantity sold, and number of orders.
- **Visual**: A KPI chart displaying total sales, profit, and quantity sold.
- **Sample Visual**: ![Total Sales KPI](path/to/visual/image)

### 2. **Sales and Profit Analysis**

- **Insight**: Analyze sales and profit by product category, region, and market.
- **Visual**: A bar chart showing sales and profit for each product category, region, or market.
- **Sample Visual**: ![Sales and Profit Analysis](path/to/visual/image)

### 3. **Category-wise Profit**

- **Insight**: Break down the profit contribution of each product category.
- **Visual**: A pie chart showing profit distribution across product categories.
- **Sample Visual**: ![Category-wise Profit](path/to/visual/image)

### 4. **Segment-wise Sales Share**

- **Insight**: Understand the distribution of sales across different customer segments (e.g., Consumer, Corporate).
- **Visual**: A stacked bar chart showing sales share by segment.
- **Sample Visual**: ![Segment-wise Sales Share](path/to/visual/image)

### 5. **Sales by Country**

- **Insight**: Visualize sales performance by country to identify key markets.
- **Visual**: A map chart or bar chart showing sales by country.
- **Sample Visual**: ![Sales by Country](path/to/visual/image)

### 6. **Top 5 Subcategories**

- **Insight**: Identify the best-performing subcategories based on sales or profit.
- **Visual**: A bar chart showing the top 5 subcategories based on sales or profit.
- **Sample Visual**: ![Top 5 Subcategories](path/to/visual/image)

### 7. **Bottom 5 Subcategories**

- **Insight**: Identify underperforming subcategories for further analysis and possible improvements.
- **Visual**: A bar chart showing the bottom 5 subcategories based on sales or profit.
- **Sample Visual**: ![Bottom 5 Subcategories](path/to/
