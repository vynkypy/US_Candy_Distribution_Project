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
## Key Highlights:
- KPIs at a Glance: Track Total Sales, Units Sold, Profit Margins, Delivery Times, and Target Achievement in one view.
- Sales Trends: Visualize monthly sales performance and growth trajectory across years.
- Target vs Actual: Compare division-wise performance against strategic targets.
- Geographical Insights: Map-based view of sales distribution and factory locations for better spatial awareness.
- Factory Analytics: Understand which factories drive the most gross profit and product output.
- Top Products: Dive into the best-selling and most profitable products with combined bar & line visuals

---
## 📐 Key Metrics & DAX Measures

- **Total Sales**, **Total Units**, **Gross Profit**, **Cost**
- **Avg Delivery Days**
- **Slicers for dynamic filtering by Year, Division, Region, Factory, and more**

  ```dax
  Avg Delivery Days = AVERAGEX(Sales, DATEDIFF(Sales[Order Date], Sales[Ship Date], DAY))

💡 ## Biggest Takeaway:
This project was not just about building a dashboard - it was a deep learning experience in data modeling, DAX optimization, and translating raw datasets into meaningful business narratives.The biggest lesson? Good analytics isn’t just about numbers - it’s about storytelling that drives action.
