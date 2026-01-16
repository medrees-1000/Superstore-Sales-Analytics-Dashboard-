# Superstore Sales Analytics Dashboard

##  Project Overview
This project delivers an end-to-end sales and profitability analysis for a retail superstore using **SQL** and **Power BI**.  
The goal was to move beyond static spreadsheets and build a scalable, query-driven analytics pipeline that supports executive-level decision-making.

A SQL-based semantic layer was engineered to power an interactive dashboard that highlights revenue trends, profitability drivers, regional performance, and the financial impact of discounting strategies.

---

##  Business Problem
Retail leadership needed a clear understanding of:
- Which product categories and regions drive profitability
- How discounting affects margins
- Why high sales volume does not always translate to high profit
- How performance trends evolve over time

---

##  Dashboard Preview
![Dashboard Preview](screenshots/dashboard_preview.png)

---

##  Tech Stack
* **Data Source:** Kaggle – Superstore Sales (Final)
* **Data Preparation:** Microsoft Excel (data cleaning & formatting)
* **Database:** SQLite
* **Query Language:** SQL
* **Visualization:** Power BI
* **Version Control:** Git & GitHub

---

## Project Architecture
```text
superstore-sales-analytics/
│
├── data/
│   ├── Sample - Superstore Original.csv
│   └── Superstore Cleaned.csv
│
├── sql/
│   ├── create_table.sql
│   ├── Kpi_queries.sql
│   └── create_views.sql
│
├── dashboard/
│   └── Superstore_Sales_Dashboard.pbix
│
├── screenshots/
│   └── dashboard_preview.png
│
├── docs/
│   └── data_dictionary.md
│
└── README.md
```
---

## Key Analytical Insights
- Generated **$2.3M in total sales** with a **12.47% profit margin** across four years (2014–2017).
- Identified **Technology** as the most profitable category, while **Furniture** underperformed despite strong sales volume.
- Revealed that **high discount levels (31%–50% and 50%+) consistently resulted in net losses**, especially in the Tables sub-category.
- Demonstrated that **high sales do not guarantee high profit**, with several sub-categories generating revenue at a loss.
- Regional analysis showed the **West and East regions** as top contributors to revenue and profit.

---

## SQL Semantic Layer
To improve performance and reusability, the dashboard is powered by a SQL semantic layer composed of analytical views:
- `vw_overall_kpis` – Executive KPIs (Sales, Profit, Margin)
- `vw_monthly_performance` – Time-series trends
- `vw_region_performance` – Geographic analysis
- `vw_category_performance` – Category-level profitability
- `vw_discount_impact` – Discount vs. profit diagnostics

This approach separates business logic from visualization, enabling scalable analytics.

---

##  How to Run This Project
1. Load `superstore.csv` into SQLite using the schema in `create_table.sql`.
2. Execute SQL scripts in the `/sql` folder to create analytical views.
3. Open `superstore_dashboard.pbix` in Power BI.
4. Refresh data connections if needed.

---

##  Why This Project Matters
This project demonstrates:
- Strong SQL fundamentals and data modeling
- Business-focused analytical thinking
- Clean dashboard design for executive audiences
- An end-to-end analytics workflow similar to real-world BI teams

---

##  License
This project is licensed under the MIT License.
