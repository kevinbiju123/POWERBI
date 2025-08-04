
---

## 📄 README Format 2: **Business Case + Insights Driven**

markdown
# 📈 Business Optimization Dashboard using Power BI

An end-to-end analytics project that leverages sales and inventory data to help optimize business operations by identifying supply shortages, demand surges, and financial impact across multiple electronic products.

---

## 🧩 Problem Statement

The business lacked visibility into real-time product demand vs availability, leading to lost sales and overstocking. There was no central system to quantify profit/loss per product and assess performance across categories.

---

## 💡 Solution

We developed a multi-source Power BI dashboard powered by **SQL Server** (Test/Production) and **MySQL** data that:
- Tracks average daily demand and availability.
- Calculates total supply shortages.
- Quantifies profit and loss based on unit price and daily stock movement.
- Allows drill-downs by product (e.g., TV, Laptop, Air Purifier).

---

## 📊 Key KPIs Tracked

| KPI                        | Value     |
|----------------------------|-----------|
| Average Demand per Day     | 3,724     |
| Average Availability per Day | 2.87    |
| Total Supply Shortage      | 579 units |
| Total Profit               | 21.53K    |
| Total Loss                 | -97.37K   |
| Average Daily Loss         | -88.84    |

---

## 📍 Insights Uncovered

- Products like **Action Cameras** and **Bluetooth Headphones** had the **highest demand but lowest availability**, driving major losses.
- **Supply shortages** are responsible for a consistent **negative daily loss**, suggesting restocking is not aligned with demand patterns.
- **Profit** was primarily driven by a few well-supplied SKUs, while most others incurred heavy loss due to missed availability.

---

## ✅ Business Impact

- Highlighted exact SKUs needing inventory prioritization.
- Supported smarter restocking strategies.
- Quantified loss from unavailability—enabling C-level stakeholders to approve operational changes.

---

## 🛠 Tools Used

- **SQL Server** (Test & Production)
- **MySQL Database**
- **Power BI Desktop & Service**
- **DAX, M Query, Advanced Editor**

---

## 🌐 Deployment

Final report published to Power BI Service using both **SQL Server** and **MySQL** data sources for real-time updates.

