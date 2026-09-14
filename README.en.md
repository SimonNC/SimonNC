# 👋 Simon Jorite | Data Analyst
[🇫🇷 Version française](README.md)

Certified **[Microsoft Power BI Data Analyst (PL-300)](https://learn.microsoft.com/en-us/users/simonjorite-4846/credentials/b2cc3310a92a9302)** with 15 years of hands-on experience in finance, operations, and e-commerce. I bridge business expertise with production-grade analytics - transforming complex datasets into reliable KPIs and decision-ready dashboards.

---

### 🎯 Professional Positioning

**Data Analyst with a dual data & finance background.**

Most data analysts come from engineering or statistics. I come from the business side - controlling, payments, fraud analytics, multi-country operations - and built my technical stack (SQL, Power BI, Python, dbt) on top of that foundation.

This means I don't just deliver dashboards. I understand the decisions they need to support.

- **Business-first approach**: I start from the operational question, not the tool. Every KPI I design has a clear owner and a concrete use case.
- **Production-grade mindset**: I treat data as a product - layered architectures (`staging` to `marts`), automated testing, CI/CD, documentation.
- **Proven impact**: ~15% fraud loss reduction across 30 countries (Betclic), ~167 hours saved through Python automation (RHPro), 64% of negative reviews traced to a single logistics bottleneck (Olist project).

---

### 🛠️ Technical Stack

| Domain | Tools & Skills |
|---|---|
| **Data Analysis & BI** | SQL (PostgreSQL, BigQuery), Power BI (DAX, Power Query, Star-Schema), KPI design, data visualization |
| **Analytics Engineering** | dbt (staging/marts, data contracts, CI/CD), data modeling (fact/dimension), automated documentation |
| **Python & Automation** | Pandas, NumPy, Scikit-learn, API REST, web scraping, n8n workflow orchestration |
| **Cloud & Infrastructure** | BigQuery, Fivetran (fundamentals), Airflow (fundamentals), Docker, Git/GitHub Actions |
| **Business Verticals** | Finance & controlling, payments & fraud analytics, e-commerce operations, multi-country reporting |

---

### 🚀 Featured Projects

#### 1. [E-commerce Performance Analysis - Olist](https://github.com/SimonNC/olist-data-analysis)

> **Key insight: 64% of negative reviews are linked to deliveries exceeding 30 days.**

<p align="center">
  <a href="https://github.com/SimonNC/olist-data-analysis">
    <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/reviews_dashboard.jpg" alt="Olist Reviews Dashboard - Power BI" width="720"/>
  </a>
</p>

- **Context**: Large-scale e-commerce dataset with no clear view of what drives customer satisfaction.
- **What I did**: Built a reproducible Python pipeline (cleaning, feature engineering, quality checks), then designed a Power BI Star-Schema model to surface logistics KPIs.
- **Tech**: Python (Pandas), SQL, Power BI (DAX, Power Query).
- **Impact**: Identified the 30-day delivery threshold as the dominant satisfaction driver. Delivered actionable KPIs for logistics prioritization.

<details>
<summary>📊 More dashboards from this project</summary>
<br/>
<p align="center">
  <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/sales_dashboard.jpg" alt="Olist Sales Dashboard" width="680"/>
</p>
<p align="center"><em>Sales Performance Dashboard - Revenue trends, top categories & regions</em></p>
<br/>
<p align="center">
  <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/delivery_dashboard.jpg" alt="Olist Delivery Dashboard" width="680"/>
</p>
<p align="center"><em>Delivery & Logistics Dashboard - SLA distribution & on-time rate</em></p>
<br/>
<p align="center">
  <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/data_model.jpg" alt="Olist Data Model" width="680"/>
</p>
<p align="center"><em>Star-Schema Data Model - Power BI</em></p>
</details>

---

#### 2. [Analytics Engineering Pipeline - dbt](https://github.com/SimonNC/olist-dbt-duckdb)

> **12 dbt models with data contracts and automated CI/CD.**

```
Raw Data  ──►  Staging  ──►  Intermediate  ──►  Marts (BI-Ready)
                                                  ├── Revenue
                                                  └── Retention
                 dbt tests as data contracts
                 GitHub Actions CI/CD at every commit
```

- **Context**: Fragmented raw data leading to inconsistent KPI reporting. Goal: build a reliable, layered data warehouse architecture.
- **What I did**: Designed a multi-layer dbt project (`staging`, `intermediate`, `marts`) with controlled grains. Implemented dbt tests as data contracts and GitHub Actions for automated CI/CD and documentation.
- **Tech**: SQL, dbt Core, GitHub Actions. Built with DuckDB for local development; architecture designed to port to cloud warehouses (BigQuery, Snowflake).
- **Impact**: Delivered BI-ready marts for Revenue and Retention analysis. Established a Single Source of Truth with automated quality enforcement.

---

#### 3. [Customer Churn Prediction - Telco](https://github.com/SimonNC/telco-customer-churn-prediction)

> **ML decision-support tool: 0.84 ROC-AUC, 0.73 recall on churners.**

```
 7,043 customers
      │
 Business-oriented EDA ──► Key churn drivers identified
      │
 Leakage-safe ML pipeline (recall-first)
      │
 Streamlit app ──► Simulate retention strategies in real time
```

- **Context**: Customer churn as a major financial risk in telecom - acquisition costs far exceed retention costs.
- **What I did**: Conducted business-oriented EDA on 7,043 customers to identify key churn drivers. Built a leakage-safe ML pipeline with a recall-first strategy. Deployed a Streamlit app for customer profile simulation and threshold tuning.
- **Tech**: Python (Pandas, Scikit-learn), Random Forest, Logistic Regression, Streamlit, Git/GitHub.
- **Impact**: Actionable tool enabling business teams to identify at-risk customers early and simulate retention strategies based on real-time churn probabilities.

---

### 📜 Certifications

| Certification | Status |
|---|---|
| [Microsoft PL-300 - Power BI Data Analyst Associate](https://learn.microsoft.com/en-us/users/simonjorite-4846/credentials/b2cc3310a92a9302) | Certified (2025) - [Verify credential](https://learn.microsoft.com/en-us/users/simonjorite-4846/credentials/b2cc3310a92a9302) |
| Le Wagon - Data Analytics Bootcamp (RNCP Level 6) | Certified (2025) |
| AWS Solutions Architect - Associate | In progress |
---

### 🌍 Languages

- **French**: Native
- **English**: Fluent - 6+ years in English-speaking environments (Dublin, Malta)
- **Spanish**: Conversational

---

### 📫 Contact & Opportunities

- **LinkedIn**: [linkedin.com/in/simonjorite](https://www.linkedin.com/in/simonjorite)
- **Email**: simon.jorite@gmail.com
- **Scheduling**: [Book a 30-min exchange](https://calendly.com/simon-jorite/echange-da)
- **Location**: Lyon, France - Open to hybrid / remote
