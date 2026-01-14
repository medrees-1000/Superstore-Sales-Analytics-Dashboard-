# Superstore Sales Analytics Dashboard

##  Project Overview
This project provides a comprehensive analysis of retail sales data to identify key drivers of profitability and sales growth. By moving beyond simple spreadsheets, I engineered a robust SQL-based data pipeline to power an interactive Business Intelligence dashboard.

##  Tech Stack
* **Data Source:** Kaggle Superstore Sales (Final)
* **Database:** SQLite
* **Data Engineering:** SQL (Views, CASE Statements, Date Normalization)
* **Visualization:** [Power BI / Tableau] - *Coming Soon*

##  Key Business Insights (Verified)
* **Total Revenue:** $2,297,201.07
* **Total Profit:** $286,397.79 (12.47% Margin)
* **High-Loss Driver:** The "Tables" sub-category is the primary profit drain (-$17,725.59), directly correlated with an aggressive average discount of 26.1%.
* **Profit Leader:** The "Technology" category is the strongest performer, contributing $145,455.66 in profit.

##  Project Structure & Roadmap

### Phase 1: Data Understanding & Setup (Day 1)
* Analyzed 9,994 rows of transactional data.
* Defined data dictionary and identified data integrity requirements (e.g., preserving leading zeros in Postal Codes).

### Phase 2: Database Engineering (Day 2)
* Migrated raw CSV data into a relational SQLite database.
* Developed a schema optimized for analytical queries.
* Validated core KPIs against source data to ensure 100% accuracy.

### Phase 3: Semantic Layer & Views (Day 3)
* Created **6 Production-Ready Views** to centralize business logic:
    * `vw_orders_time`: Normalized time dimensions for time-series analysis.
    * `vw_discount_impact`: Categorized discounts into "buckets" to visualize margin impact.
    * `vw_category_performance`: Aggregated metrics for product hierarchy.
    * `vw_region_performance`: Geographic performance breakdown.

### Phase 4: Visualization (Day 4 - In Progress)
* Connecting SQL views to the BI tool.
* Designing an Executive Dashboard for stakeholder reporting.

##  Repository Contents
* `/data`: Raw and cleaned datasets.
* `/sql`: All scripts for table creation, KPI validation, and View engineering.
* `/docs`: Data dictionary and business logic notes.
