# 🌸 Ferns & Petals (FNP) — Sales Analysis Dashboard

End-to-end sales analysis of an FNP-style gifting business, covering **1,000 orders**, **71 products**, and **100 customers** — built to uncover revenue drivers, delivery performance, and customer behavior, and to answer 10 real business questions using Python and Power BI.


## 📌 Overview

Ferns & Petals sends gifts for occasions like Diwali, Raksha Bandhan, Holi, Valentine's Day, Birthdays, and Anniversaries. This project analyzes their order, product, and customer data to answer:

1. What is the total revenue?
2. What is the average order-to-delivery time?
3. How do monthly sales fluctuate across 2023?
4. Which products generate the most revenue?
5. How much do customers spend on average?
6. How do the top 5 products perform?
7. Which cities place the most orders?
8. Does order quantity affect delivery time?
9. How does revenue compare across occasions?
10. Which products are most popular per occasion?

## 🖼️ Dashboard

An interactive Power BI dashboard with KPI cards, trend charts, top-N breakdowns, and slicers (Occasion, Order Date, Delivery Date).

**Key metrics:**
| Metric | Value |
|---|---|
| Total Orders | 1,000 |
| Total Revenue | ₹35,20,984 |
| Avg. Order-to-Delivery Time | 5.53 days |
| Avg. Customer Spend | ₹35,209.84 |

## 🔑 Key Insights

- **Seasonality drives revenue** — February and August are the strongest months, aligned with Valentine's Day and festive/Raksha Bandhan buying.
- **Anniversary & Raksha Bandhan** are the top revenue-generating occasions; Diwali and Valentine's Day underperform despite being major gifting occasions.
- **Order quantity has ~0 correlation with delivery time** (r ≈ 0.003) — delivery duration is driven by other factors (city, courier, timing), not order size.
- **Top 5 products** (Magnam Set, Quia Gift, Dolores Gift, Harum Pack, Deserunt Box) contribute ~15% of revenue from just 7% of the catalog.
- **Order volume is spread across Tier-2/3 cities** rather than concentrated in metros.

## 🛠️ Tools & Tech Stack

- **Python** (Pandas) — data cleaning, joins, aggregation, correlation analysis
- **Power BI** — interactive dashboard, DAX measures, slicers
- **DAX** — Total Revenue, Avg Order-Delivery Time, Avg Customer Spend

## 📂 Repository Structure

```
├── data/
│   ├── customers.csv
│   ├── orders.csv
│   └── products.csv
├── FNP_Sales_Analysis.pbix          # Power BI dashboard file
├── FNP_Sales_Analysis_Report.docx   # Written analysis report
├── dashboard_preview.png            # Dashboard screenshot
└── README.md
```

## 📊 Methodology

1. Loaded and cleaned `orders.csv`, `products.csv`, `customers.csv` in Pandas.
2. Joined Orders ⋈ Products on `Product_ID`.
3. Derived `Revenue = Quantity × Price` and `Delivery_Days = Delivery_Date − Order_Date`.
4. Aggregated by month, product, city, category, and occasion to answer each business question.
5. Rebuilt the same logic as DAX measures in Power BI for a live, filterable dashboard.

## 👤 Author

**Aniket Kalushe**
[LinkedIn](https://linkedin.com/in/aniket-kalushe-92005431a) · [GitHub](https://github.com/Aniket-AI9075)
