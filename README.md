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
  - [1. Total Sales, Profit, Quantity, and Number of Orders](#1-total-sales-profit-quantity-and-number-of-orders)
  - [2. Sales and Profit Analysis](#2-sales-and-profit-analysis)
  - [3. Category-wise Profit](#3-category-wise-profit)
  - [4. Segment-wise Sales Share](#4-segment-wise-sales-share)
  - [5. Sales by Country](#5-sales-by-country)
  - [6. Top 5 Subcategories](#6-top-5-subcategories)
  - [7. Bottom 5 Subcategories](#7-bottom-5-subcategories)
  - [8. Yearly Sales Trend](#8-yearly-sales-trend)
- [Dashboard Features](#dashboard-features)
- [Steps to Create the Dashboard](#steps-to-create-the-dashboard)
- [Future Steps](#future-steps)
- [Significance](#Significance)
- [Adding-Visuals](#adding-visuals)

---

## Tables Used

The dashboard integrates data from the following tables, each representing a key aspect of retail operations. These tables are hosted on GitHub and connected to the Excel file using **Power Query**.

### 1. **Orders Table**

The **Orders Table** contains detailed information about each customer order, including shipping details, product categories, sales, and profit.

#### Sample Data for Orders Table:

| Row ID | Order ID           | Order Date | Ship Date  | Ship Mode    | Customer ID | Customer Name  | Segment  | City         | State   | Country     | Postal Code | Market | Region | Product ID         | Category   | Sub-Category | Product Name                                      | Sales   | Quantity | Discount | Profit  | Shipping Cost | Order Priority |
|--------|--------------------|------------|------------|--------------|-------------|-----------------|----------|--------------|---------|-------------|-------------|--------|--------|--------------------|------------|--------------|--------------------------------------------------|---------|----------|----------|--------|---------------|----------------|
| 32298  | CA-2012-124891     | 31-07-2020 | 31-07-2020 | Same Day     | RH-19495    | Rick Hansen     | Consumer | New York City| New York| United States| 10024       | US     | East   | TEC-AC-10003033     | Technology | Accessories   | Plantronics CS510 - Wireless Headset            | 2309.65 | 7        | 0        | 762.18 | 933.57        | Critical       |
| 26341  | IN-2013-77878      | 05-02-2021 | 07-02-2021 | Second Class | JR-16210    | Justin Ritter   | Corporate| Wollongong   | NSW     | Australia   | -           | APAC   | Oceania| FUR-CH-10003950     | Furniture  | Chairs        | Novimex Executive Leather Armchair, Black       | 3709.40 | 9        | 0.1      | -288.77| 923.63        | Critical       |

---

### 2. **Return Table**

The **Return Table** contains data on product returns, including the order ID and the market where the return occurred.

#### Sample Data for Return Table:

| Returned | Order ID          | Market  |
|----------|-------------------|---------|
| Yes      | MX-2013-168137    | LATAM   |
| Yes      | US-2011-165316    | LATAM   |
| Yes      | ES-2013-1525878   | EU      |
| Yes      | CA-2013-118311    | United States |
| Yes      | ES-2011-1276768   | EU      |

---

### 3. **People Table**

The **People Table** contains information about employees or key personnel and their corresponding regions.

#### Sample Data for People Table:

| Person           | Region         |
|------------------|----------------|
| Anna Andreadi    | Central        |
| Chuck Magee      | South          |
| Kelly Williams   | East           |
| Matt Collister   | West           |
| Deborah Brumfield| Africa         |

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

### 1. **Total Sales, Profit, Quantity, and Number of Orders and Profit Margin**

#### Steps to Solve:
1. **PivotTable**: Create a PivotTable to sum the **Sales**, **Profit**, and **Quantity** columns, and count the number of **Order IDs**.
2. **KPIs**: Use the **Sum of Sales**, **Sum of Profit**, and **Sum of Quantity** fields to generate the KPIs for these metrics.
3. **Dynamic Chart**: Create a dynamic KPI chart that updates automatically when new data is added.
4. **Final Output**: Display the KPIs on the dashboard, representing total sales, profit, quantity, and number of orders.

**Sample Visual**: 

![image](https://github.com/user-attachments/assets/f2166406-745f-4509-a216-0e849228281a)



### 2. **Sales and Profit Analysis**

#### Steps to Solve:
1. **PivotTable**: Create a PivotTable that groups data by **Category** (or **Region**) and calculates **Total Sales** and **Total Profit**.
2. **Bar Chart**: Plot a bar chart for **Sales** and **Profit** side by side for each category or region.
3. **Analysis**: Add slicers for the **Segment** and **Market** to filter the data for a more granular view.
4. **Final Output**: Display the chart showing sales and profit by category or region.

**Sample Visual**:

![image](https://github.com/user-attachments/assets/ba5f0a35-b50c-47d3-8df0-9ef322e5ce2f)


### 3. **Category-wise Profit**

#### Steps to Solve:
1. **PivotTable**: Group the data by **Category** and sum the **Profit** for each category.
2. **Pie Chart**: Create a pie chart to visualize the profit distribution by category.
3. **Final Output**: Display the pie chart on the dashboard, showing the percentage of profit by category.

**Sample Visual**:

![image](https://github.com/user-attachments/assets/a3bf12d8-56f4-4750-a145-8ccc50a17324)


### 4. **Segment-wise Sales Share**

#### Steps to Solve:
1. **PivotTable**: Group the data by **Segment** and sum the **Sales**.
2. **Stacked Bar Chart**: Use a stacked bar chart to show the share of sales by segment.
3. **Final Output**: Display the stacked bar chart on the dashboard, showing the sales distribution across segments.

**Sample Visual**:

![image](https://github.com/user-attachments/assets/8b1b4f11-c5e3-4390-b309-2f866c6f2dfb)

### 5. **Sales by Country**

#### Steps to Solve:
1. **PivotTable**: Group the data by **Country** and sum the **Sales**.
2. **Map Chart**: Create a map chart (or bar chart) that visualizes sales by country.
3. **Final Output**: Display the chart on the dashboard to show sales distribution across countries.

**Sample Visual**:

![image](https://github.com/user-attachments/assets/a486c52d-c82e-4017-b10b-1ed966f01346)


### 6. **Top 5 Subcategories**

#### Steps to Solve:
1. **PivotTable**:

 Group the data by **Sub-Category** and sum the **Sales**.
2. **Top N Filter**: Apply a filter to show the **Top 5 Subcategories** based on total sales.
3. **Bar Chart**: Create a bar chart to display the top 5 subcategories.
4. **Final Output**: Display the bar chart on the dashboard showing the top 5 subcategories.

**Sample Visual**:

![image](https://github.com/user-attachments/assets/7ea11e17-7f3f-4ccd-b873-273f99887c91)

### 7. **Bottom 5 Subcategories**

#### Steps to Solve:
1. **PivotTable**: Group the data by **Sub-Category** and sum the **Sales**.
2. **Bottom N Filter**: Apply a filter to show the **Bottom 5 Subcategories** based on total sales.
3. **Bar Chart**: Create a bar chart to display the bottom 5 subcategories.
4. **Final Output**: Display the bar chart on the dashboard showing the bottom 5 subcategories.

**Sample Visual**:

![image](https://github.com/user-attachments/assets/54823a4a-aa2b-4c6e-b8b5-f8aaed0c123b)


### 8. **Yearly Sales Trend**

#### Steps to Solve:
1. **PivotTable**: Group the data by **Order Date** and sum the **Sales**.
2. **Line Chart**: Plot a line chart to show the sales trend over the years.
3. **Final Output**: Display the line chart on the dashboard showing yearly sales trends.

**Sample Visual**:

													
													
![image](https://github.com/user-attachments/assets/8aa96c3b-5d86-43d1-a9ec-0ae7eb896a11)



## Dashboard Features

- **Interactive Charts**: Dynamic charts that update based on user selection from filters (e.g., Region, Segment, Market).
- **Dynamic KPIs**: Displays total sales, profit, quantity, and profit margin with real-time updates.
- **Yearly Trends**: Visualizes sales trends by year to help forecast future performance.
- **Category and Subcategory Breakdown**: Detailed analysis of sales and profits by category and subcategory.

---

## Steps to Create the Dashboard

1. **Prepare the Data**:
   - Load the **Orders**, **Returns**, and **People** tables into Excel via **Power Query**.
   - Perform necessary data transformations (e.g., data type adjustments, removing duplicates).
   - Link the tables using relationships (if required).

2. **Create PivotTables**:
   - For each analysis, create a PivotTable to aggregate the data based on specific dimensions (e.g., Category, Segment, Country).
   - Use **Slicers** to allow filtering by key attributes like **Region**, **Market**, and **Segment**.

3. **Design the Dashboard Layout**:
   - Place the KPIs at the top for a quick overview.
   - Arrange the charts for each analysis below the KPIs.
   - Use dynamic **chart titles** and **data labels** to reflect the filter selections.

4. **Add Interactivity**:
   - Add **Slicers** and **Timeline** controls to make the dashboard dynamic.
   - Set up **Conditional Formatting** to highlight key values.

5. **Test the Dashboard**:
   - Ensure the dynamic charts and KPIs update correctly when applying filters.

---

## Future Steps

- **Return Analysis**: Add a section to analyze the return rate by product, region, and market.
- **Top and Bottom Customers**: Display the top and bottom customers based on sales or profit.
- **Segment and Market Analysis**: Provide insights into how each market and segment is performing.

---

## Significance

- Track perforamance through KPIs.
- Undestand category, segment, and geographic trends.
- Made data-driven decisions to optimize operations.
  
---
## Visuals
- Visuals example for each solved problem statement.
- Snapshots of the final Dashboard with all components.

![Dashboard](https://github.com/user-attachments/assets/ae53b07d-17fc-456e-b6f8-0f020a5131b6)
