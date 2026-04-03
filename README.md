
# 📊 Sales Analytics Dashboard Project

## 🚀 Overview

This project focuses on analyzing sales data and building an interactive dashboard using **SQL + Power BI**. It involves data cleaning, transformation, querying, and visualization to generate meaningful business insights.

---

## 📁 Project Structure

```
├── sales_raw_500.xlsx      # Raw dataset
├── sales_cleaned.csv       # Cleaned dataset
├── Dashboard.pbix          # Power BI dashboard file
├── sql_queries.sql         # SQL queries used for analysis
└── README.md               # Project documentation
```

---

## 🛠️ Technologies Used

* **SQL (MySQL / PostgreSQL)** – Data querying & analysis
* **Excel** – Data preprocessing
* **Power BI** – Dashboard & visualization
* **Python (Optional)** – Data cleaning (Pandas, NumPy)

---

## 📌 Features

* 📈 Sales trend analysis (monthly/yearly)
* 🧑‍💼 Customer segmentation
* 🌍 Region-wise performance
* 💰 Revenue & profit analysis
* 🧠 SQL-based insights extraction
* 📊 Interactive dashboard

---

## 🧹 Data Cleaning Steps

* Removed null/missing values
* Removed duplicate records
* Standardized column names
* Converted date formats
* Exported cleaned data into CSV

---

## 🧠 SQL Analysis

Key SQL queries used:

### 🔹 Total Sales

```sql
SELECT SUM(Sales) AS Total_Sales FROM sales;
```

### 🔹 Region-wise Sales

```sql
SELECT Region, SUM(Sales) AS Total_Sales
FROM sales
GROUP BY Region
ORDER BY Total_Sales DESC;
```

### 🔹 Top 5 Products

```sql
SELECT Product_Name, SUM(Sales) AS Revenue
FROM sales
GROUP BY Product_Name
ORDER BY Revenue DESC
LIMIT 5;
```

### 🔹 Monthly Sales Trend

```sql
SELECT MONTH(Order_Date) AS Month, SUM(Sales) AS Total_Sales
FROM sales
GROUP BY Month
ORDER BY Month;
```

---

## 📊 Dashboard Insights

The Power BI dashboard provides:

* Total Sales, Profit & Quantity KPIs
* Monthly trends visualization
* Top products & categories
* Region-wise comparison

---

## ▶️ How to Use

1. Clone/download this repository
2. Run SQL queries on your database
3. Open `Dashboard.pbix` in Power BI
4. Load cleaned dataset
5. Explore dashboard

---


## 🎯 Use Cases

* Data Analyst portfolio project
* Business performance analysis
* SQL + BI integration practice

---

