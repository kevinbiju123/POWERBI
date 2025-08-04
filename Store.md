# 📊 Sales and Returns Dashboard – Power BI Project

This repository contains an interactive Power BI dashboard developed to analyze sales performance, customer profitability, product trends, and returns using datasets from a retail business. The dashboard visualizes key metrics across segments, regions, and time periods to support data-driven decision-making.

---

## 🧩 Problem Statement

The company lacks a centralized, visual system to monitor and analyze its sales, returns, and customer behavior across different segments and markets. Without a comprehensive view, it's difficult to identify profitable customers, high- and low-performing products, regional sales trends, and the root causes of return orders. This limits the organization’s ability to make data-driven decisions for improving profitability, streamlining operations, and refining market strategy. The goal is to develop a Power BI dashboard to consolidate this information and uncover actionable insights.

---

## 📂 Datasets Used

| File Name      | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `Orders.xlsx`  | Contains transactional data (Order ID, Sales, Quantity, Segment, Region)    |
| `People.xlsx`  | Maps salespeople to their corresponding regions                             |
| `Returns.xlsx` | Contains information about returned orders (Order ID)                       |

---

## ⚙️ Steps Followed

1. **Data Cleaning & Integration**
   - Merged `Orders` and `Returns` using `Order ID` to track returned orders.
   - Joined `People` dataset with regional information to identify responsible personnel.

2. **Data Transformation**
   - Created measures for Total Sales, Quantity Sold, Average Delivery Days, and Return Orders.
   - Applied DAX functions to categorize data by Year, Segment, and Market.

3. **Visualization Design**
   - KPIs: Sales, Quantity, Delivery Days, Return Count.
   - Pie & donut charts: Sales by Segment and Market.
   - Map: Regional sales distribution using Bing Maps.
   - Bar charts: Top Customers by Profit, Top/Bottom Products.

---

## 📈 Dashboard KPIs

| Metric               | Value    |
|----------------------|----------|
| Total Sales          | $4.30M   |
| Quantity Sold        | 61K      |
| Average Delivery Days| 4        |
| Total Return Orders  | 1,079    |

---

## 🔍 Key Insights

- **Sales Segments:**  
  Consumer segment led with **$2.14M**, nearly **50% of total sales**.

- **Top Markets:**  
  Asia Pacific ($1.37M) and Europe ($1.18M) dominate the market share.

- **Customer Profitability:**  
  Ray was the top customer contributing **$7.4K** in profit.

- **Product Profitability:**  
  *Canon imageCLASS* products generated the highest profit (**$16K**), followed by Cisco and Motorola.

- **Loss-making Products:**  
  *Cubify Cube* had the highest loss (**-$3.8K**), highlighting inventory or pricing issues.

- **Return Volumes:**  
  Over 1,000 return orders signal potential fulfillment, product quality, or customer experience issues.

---

## 🌍 Geographical Trends

- The dashboard uses **Bing Maps** to highlight sales by region across **North America**, **Europe**, **Asia**, and **Africa**.
- Provides a global overview to help identify strategic regional growth opportunities.

---

## ✅ Conclusions

This Power BI dashboard consolidates and visualizes sales and return data, offering actionable insights to:
- Improve customer targeting
- Optimize product inventory
- Reduce returns
- Focus marketing and sales efforts on high-performing regions and products
