# 🍭 Candy Distributor Analytics Dashboard

This project delivers a comprehensive and interactive Power BI dashboard designed for a fictional U.S.-based candy distributor. The dashboard enables rich insights into sales, customer behavior, factory performance, shipping efficiency, and geographic trends.

---

## 📊 Project Overview

**Objective:**  
To analyze sales and operational data across multiple dimensions (product, region, factory, customer, etc.) and present insights using an eye-catching, user-friendly Power BI dashboard.

---

## Data Sources

| Table       | Description                                        |
|-------------|----------------------------------------------------|
| `Sales`     | Transaction-level sales data (10,000+ records)     |
| `Products`  | Product metadata, pricing, cost, factory info      |
| `Factories` | Factory geolocation data (lat/lng)                 |
| `Targets`   | Sales targets by product division (for 2024)       |
| `US Zips`   | U.S. ZIP code data (geo, population, timezone etc.)|

---

## 📐 Key Metrics & DAX Measures

- **Total Sales**, **Total Units**, **Gross Profit**, **Cost**
- **Avg Delivery Days**  
  ```dax
  Avg Delivery Days = AVERAGEX(Sales, DATEDIFF(Sales[Order Date], Sales[Ship Date], DAY))
