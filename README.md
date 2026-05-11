# Adidas Sales Analysis Dashboard

## 📌 Project Overview
The Adidas Sales Analysis project was developed using Power BI to analyze Adidas US sales data and generate insights related to revenue, profitability, product performance, and regional sales trends. The dashboard helps management monitor performance and support data-driven decision-making.

---

## 🎯 Project Objective & Scope of Work

### Objectives
- Analyze Adidas sales performance
- Identify profitable products and regions
- Track sales and profit trends
- Create interactive dashboards using Power BI

### Scope of Work
- Data cleaning and transformation
- Data modeling and DAX calculations
- KPI and dashboard development
- Business insights generation

---

## 🗂️ Data Source & Architecture

### Data Source
- **Source:** Adidas US Sales Dataset (.xlsx)
- **Records:** 9,648
- **Columns:** 13

### Architecture
```text
Excel Dataset → Power Query → Data Model → DAX Measures → Dashboard
```

---

## ⚙️ Implementation Steps

1. Imported Excel dataset into Power BI
2. Cleaned and transformed data using Power Query
3. Created Date Table and relationships
4. Developed DAX measures and KPIs
5. Designed interactive dashboard pages
6. Added slicers, navigation, and interactivity

---

## 🧩 Data Modelling

### Tables Used
- **Fact Table:** Data Sales Adidas
- **Dimension Table:** Date Table

### Relationship
```text
Date Table[Date] → Sales Table[Invoice Date]
```

---

## 📊 DAX Measures

```DAX
Total Revenue =
SUM('Data Sales Adidas'[Total Sales])

Total Profit =
SUM('Data Sales Adidas'[Operating Profit])

Total Units Sold =
SUM('Data Sales Adidas'[Units Sold])

Profit Margin % =
DIVIDE([Total Profit], [Total Revenue])

Sales LY =
CALCULATE(
    [Total Revenue],
    SAMEPERIODLASTYEAR('Date Table'[Date])
)

Sales Growth % =
DIVIDE([Total Revenue] - [Sales LY], [Sales LY])

Avg Price Per Unit =
AVERAGE('Data Sales Adidas'[Price per Unit])
```

---

## 🖥️ Dashboard Pages Summary

### 🏠 Index Page
- Dashboard navigation page
- Adidas branding and page routing

### 📈 Executive Overview
- Revenue and profit KPIs
- Sales trend analysis
- Revenue by region and sales method

### 👟 Product Performance
- Product revenue and profit analysis
- Units sold by product and retailer
- Product ranking analysis

### 🌍 Regional Analysis
- Region-wise sales analysis
- State-level performance
- Regional profit insights

---

## 🎛️ Filters & Interactivity

### Slicers Used
- Year
- Month
- Product
- Retailer
- Region

### Features
- Cross filtering
- Interactive visuals
- Navigation buttons
- Dynamic analysis

---

## 💡 Key Insights

- West region generated the highest revenue
- Men’s Street Footwear was the top-performing product
- In-store sales contributed maximum revenue
- New York and California were top-performing states
- Revenue and profit showed strong growth trends

---

## ✅ Conclusion

The Adidas Sales Analysis dashboard successfully transformed raw sales data into a professional and interactive reporting solution. The dashboard provides valuable insights into sales, profitability, products, and regional performance, helping support strategic business decisions.

---

## 📸 Dashboard Screenshots

### 🏠 Index Page
_<img width="1366" height="768" alt="Index" src="https://github.com/user-attachments/assets/d20efa59-19da-4c3a-9208-74e45b1e9b30" />_

### 📈 Executive Overview
_<img width="1366" height="768" alt="EO" src="https://github.com/user-attachments/assets/3eaddb52-30f4-437f-b038-a197ac246f3e" />_

### 👟 Product Performance
_<img width="1366" height="768" alt="Prod Perf" src="https://github.com/user-attachments/assets/5fb65e83-638a-4c0a-b728-d3cb145033ea" />
_

### 🌍 Regional Analysis
_<img width="1366" height="768" alt="Reg Anlys" src="https://github.com/user-attachments/assets/fb1ac2f1-4525-4e03-b80f-556dbcbc5809" />
_

---

## 🛠️ Tools & Technologies Used

- Power BI
- Power Query
- DAX
- Microsoft Excel

---
