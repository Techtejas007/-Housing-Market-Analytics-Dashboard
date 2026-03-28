# 🏠 Housing Market Analytics Dashboard

> A comprehensive 3-page Power BI dashboard analyzing real estate market performance — covering price trends, regional sales, house type comparisons, and key drivers of property purchase prices.

---

## 📌 Problem Statement

Real estate analysts, property consultants, and investors often struggle to:
- Understand year-over-year sales growth across different sales types
- Compare offer prices vs. actual purchase prices to spot negotiation gaps
- Identify which regions are commanding the highest price per SQM
- Understand what factors (age, area, type) most influence purchase price

This dashboard brings together all key housing market KPIs into a single, interactive analytical tool.

---

## 🖥️ Dashboard Pages

| Page | Description |
|------|-------------|
| **House Market Overview** | YOY sales growth by type, offer vs. purchase price scatter plot, median price change by region, latest quarter units sold, 12-month sales KPI |
| **Sales Performance** | Sales by region bar chart, average price per SQM donut, key drivers of purchase price, offer-to-SQM ratio by sales type |
| **House Type Analysis** | Avg offer/purchase price by house type, inflation/interest/yield comparisons, SQM vs. SQM price combo chart, slicers for area/city/sales type/region |

---

## 🔍 Key Features

- **YOY Sales Growth** — line chart showing annual growth rate by sales type
- **Offer vs. Purchase Price** scatter plot — reveals pricing negotiation gaps
- **Key Drivers visual** — AI-powered insight into what most influences purchase price (Age, Area)
- **Inflation / Interest / Yield analysis** — macro-economic overlays on house type performance
- **Dynamic slicers** — filter entire report by Area, City, Sales Type, and Region
- **KPI Cards** — instant view of units sold in latest quarter and trailing 12-month sales

---

## 🛠️ Tech Stack

| Tool | Usage |
|------|-------|
| **Power BI Desktop** | Report development and layout |
| **DAX** | YOY Growth, YTD Sales, Median Price Change, Price Per SQM, Offer-to-SQM Ratio |
| **Power Query (M)** | Data cleansing, region/type normalization |
| **Power BI Key Influencers Visual** | AI-driven driver analysis for purchase price |

---

## 📊 Key DAX Measures

```dax
YOY_Sales_Growth = 
DIVIDE([Current Year Sales] - [Prior Year Sales], [Prior Year Sales])

Average Price SQM = AVERAGE('Housing'[price_per_sqm])

Offer to SQM Ratio = DIVIDE([Average Offer Price], [Average SQM])
```

---

## 📊 Dataset Fields

`purchase_price` · `Offer Price` · `region` · `area` · `city` · `house_type` · `sales_type` · `Age` · `YOY_Sales_Growth` · `Median Sales Price Change` · `TotalYTD Sales`

---

## 💡 Business Impact

- Helps **real estate agents** identify regions with the strongest price growth for targeted listings
- Enables **property investors** to evaluate offer-to-purchase gaps across house types
- Supports **mortgage lenders** in understanding key price drivers (age, area) for risk assessment
- Gives **market analysts** macro trend data (inflation, yield, interest) alongside sales performance

---

## 📁 File

| File | Description |
|------|-------------|
| `Housing_Data.pbix` | Power BI report file |

---

## 🚀 How to Use

1. Download `Housing_Data.pbix`
2. Open in **Power BI Desktop**
3. Start on the **House Market Overview** page for a macro view
4. Use slicers on the **House Type Analysis** page to filter by city, area, or region
5. Use the action button to navigate between pages

---

## 👤 Author

**Tejas Bafna** — Data Analyst | Power BI Developer  
📧 tejasbafna311@gmail.com · [LinkedIn](https://linkedin.com) · 📍 Nashik, India
