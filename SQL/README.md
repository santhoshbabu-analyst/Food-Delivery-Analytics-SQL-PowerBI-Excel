# 🧠 SQL Analytics

This folder contains **SQL queries and analytical logic** used to build the Food Delivery Analytics system.

The SQL layer acts as the **core engine** of the project, where daily appended data is transformed into meaningful KPIs and trends for Excel and Power BI dashboards.

---

## Database Overview

- Database: `food_delivery`
- Main Table: `food_delivery_orders`
- Data Source: Daily order data from **Zomato & Swiggy**
- Data Type: Incremental (daily append)

---

## Key SQL Analyses

### 📊 Order Performance
- Daily, weekly, monthly, and YTD order counts
- Current vs previous period comparisons
- Day-over-Day (DoD), Week-over-Week (WoW), Month-over-Month (MoM)

---

### 📈 Trend Analysis
- Rolling averages (7-day, 14-day)
- Moving trends using window functions
- Longest increasing/decreasing streaks
- Seasonality and peak-time analysis

---

### 🏙 City & Area Analysis
- City-wise contribution %
- Area-wise ranking using window functions
- Top-performing and declining locations
- Peak-hour demand analysis

---

### 👥 Customer Analytics
- New vs returning customers
- Repeat customer identification
- Customer retention & cohort analysis
- Platform switching behavior (Zomato ↔ Swiggy)

---

### 🔄 Platform Comparison
- Zomato vs Swiggy order share
- Monthly platform contribution %
- Platform-wise YoY growth analysis

---

## Advanced SQL Concepts Used

- Window Functions (`ROW_NUMBER`, `RANK`, `LAG`, `LEAD`)
- CTEs (`WITH` clauses)
- Date & time functions
- Rolling aggregates
- Conditional aggregation
- Performance-optimized queries

---

## Usage
- Queries are executed daily after data append
- Outputs directly feed Excel & Power BI dashboards
- Ensures automated KPI refresh without manual intervention

📌 Files included:
- `food_delivery_analysis_queries.sql`
