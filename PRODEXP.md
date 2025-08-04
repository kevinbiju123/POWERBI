# 📊 Business Optimization Dashboard (End-to-End Power BI Project)

This project uses data from both **SQL Server (Test + Production)** and **MySQL Database** to create a business optimization dashboard that tracks demand, availability, profit, and loss for various electronic products. It includes advanced DAX calculations, ETL steps, and transition between environments.

---

## 🗂️ Files Used

### ✅ `Test Environment Inventory Dataset.csv`
- Simulates inventory data for training/test.
- Imported into SQL Server using `LEFT JOIN` queries to combine demand, availability, and pricing data.

### ✅ `Prod Env Inventory Dataset.csv`
- Final production-ready dataset.
- Imported after transformation and data validation from SQL Server.

### ✅ `Products.csv`
- Lookup table for product names and types.
- Joined with main fact table to enable filtering in Power BI.

---

## 🔄 Data Connections Used

| Environment     | Connection Type | Tool              |
|-----------------|------------------|-------------------|
| Test            | SQL Server       | Power BI Desktop  |
| Production      | SQL Server       | Power BI Desktop  |
| Final Transition| MySQL Database   | Power BI Connector (ODBC) |

Advanced Query Editor and **SQL transformations** were used to clean & validate transitions before moving to MySQL production.

---

## 🔧 DAX Measures Used

### 📦 Demand & Supply Metrics

##DAX
Total Demand = SUM('Demand/Availability'[demand])

Total Availability = SUM('Demand/Availability'[availability])

Total Number of Days = DISTINCTCOUNT('Demand/Availability'[Order_Date_DD_MM_YYYY].[Date])

Average Demand per Day = DIVIDE([Total Demand], [Total Number of Days], 0)



Average Availability Per Day = DIVIDE([Total Availability], [Total Number of Days], 0)
Total Supply Shortage = [Total Demand] - [Total Availability]


Total Profit = 
SUMX(
    FILTER('Demand/Availability', 'Demand/Availability'[Profit/Loss] > 0),
    'Demand/Availability'[Profit/Loss] * 'Demand/Availability'[unit_price]
)

Total Loss = 
SUMX(
    FILTER('Demand/Availability', 'Demand/Availability'[Profit/Loss] < 0),
    'Demand/Availability'[Profit/Loss] * 'Demand/Availability'[unit_price]
)

Average Loss Per Day = DIVIDE([Total Loss], [Total Number of Days])
