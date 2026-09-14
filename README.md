# 👋 Simon Jorite | Data Analyst
[🇬🇧 English version](README.en.md)

Certifié **[Microsoft Power BI Data Analyst (PL-300)](https://learn.microsoft.com/en-us/users/simonjorite-4846/credentials/b2cc3310a92a9302)**, avec 15 ans d'expérience en finance, opérations et e-commerce. Je fais le pont entre expertise métier et analytics de niveau production - je transforme des jeux de données complexes en KPI fiables et en tableaux de bord prêts pour la décision.

---

### 🎯 Positionnement professionnel

**Data Analyst avec un double profil data & finance.**

La plupart des data analysts viennent de l'ingénierie ou de la statistique. Je viens du métier - contrôle de gestion, moyens de paiement, lutte anti-fraude, opérations multi-pays - et j'ai construit ma stack technique (SQL, Power BI, Python, dbt) sur cette base.

Cela signifie que je ne livre pas que des dashboards. Je comprends les décisions qu'ils doivent soutenir.

- **Approche orientée métier** : je pars de la question opérationnelle, pas de l'outil. Chaque KPI que je conçois a un propriétaire clair et un cas d'usage concret.
- **Exigence de niveau production** : je traite la donnée comme un produit - architectures en couches (`staging` à `marts`), tests automatisés, CI/CD, documentation.
- **Impact prouvé** : ~15% de réduction des pertes fraude sur 30 pays (Betclic), ~167 heures économisées grâce à l'automatisation Python (RHPro), 64% des avis négatifs rattachés à un seul goulot d'étranglement logistique (projet Olist).

---

### 🛠️ Stack technique

| Domaine | Outils & compétences |
|---|---|
| **Data Analysis & BI** | SQL (PostgreSQL, BigQuery), Power BI (DAX, Power Query, Star-Schema), conception de KPI, data visualization |
| **Analytics Engineering** | dbt (staging/marts, data contracts, CI/CD), modélisation (fact/dimension), documentation automatisée |
| **Python & Automatisation** | Pandas, NumPy, Scikit-learn, API REST, web scraping, orchestration de workflows n8n |
| **Cloud & Infrastructure** | BigQuery, Fivetran (fondamentaux), Airflow (fondamentaux), Docker, Git/GitHub Actions |
| **Secteurs métier** | Finance & contrôle de gestion, moyens de paiement & fraude, opérations e-commerce, reporting multi-pays |

---

### 🚀 Projets phares

#### 1. [Analyse de performance e-commerce - Olist](https://github.com/SimonNC/olist-data-analysis)

> **Enseignement clé : 64% des avis négatifs sont liés à des livraisons dépassant 30 jours.**

<p align="center">
  <a href="https://github.com/SimonNC/olist-data-analysis">
    <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/reviews_dashboard.jpg" alt="Olist Reviews Dashboard - Power BI" width="720"/>
  </a>
</p>

- **Contexte** : jeu de données e-commerce à grande échelle, sans vision claire des facteurs de satisfaction client.
- **Ce que j'ai fait** : construit un pipeline Python reproductible (nettoyage, feature engineering, contrôles qualité), puis conçu un modèle Power BI en Star-Schema pour faire ressortir les KPI logistiques.
- **Tech** : Python (Pandas), SQL, Power BI (DAX, Power Query).
- **Impact** : identifié le seuil des 30 jours de livraison comme facteur dominant de satisfaction. KPI actionnables livrés pour prioriser la logistique.
- **Essayer** : [Ouvrir le dashboard dans Power BI](https://raw.githubusercontent.com/SimonNC/olist-data-analysis/main/exports/olist_dashboard.pbix) *(.pbix, prêt à l'emploi)*

<details>
<summary>📊 Plus de dashboards pour ce projet</summary>
<br/>
<p align="center">
  <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/sales_dashboard.jpg" alt="Olist Sales Dashboard" width="680"/>
</p>
<p align="center"><em>Dashboard Performance Commerciale - Tendances de revenu, top catégories & régions</em></p>
<br/>
<p align="center">
  <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/delivery_dashboard.jpg" alt="Olist Delivery Dashboard" width="680"/>
</p>
<p align="center"><em>Dashboard Livraison & Logistique - Distribution SLA & taux de respect des délais</em></p>
<br/>
<p align="center">
  <img src="https://github.com/SimonNC/olist-data-analysis/raw/main/screenshots/data_model.jpg" alt="Olist Data Model" width="680"/>
</p>
<p align="center"><em>Modèle de données Star-Schema - Power BI</em></p>
</details>

---

#### 2. [Pipeline Analytics Engineering - dbt](https://github.com/SimonNC/olist-dbt-duckdb)

> **12 modèles dbt avec data contracts et CI/CD automatisée.**

```
Données brutes  ──►  Staging  ──►  Intermediate  ──►  Marts (prêts pour la BI)
                                                        ├── Revenu
                                                        └── Rétention
                        Tests dbt utilisés comme data contracts
                        CI/CD GitHub Actions à chaque commit
```

- **Contexte** : données brutes fragmentées entraînant un reporting KPI incohérent. Objectif : construire une architecture de data warehouse en couches, fiable.
- **Ce que j'ai fait** : conçu un projet dbt multi-couches (`staging`, `intermediate`, `marts`) avec des grains maîtrisés. Mis en place des tests dbt comme data contracts et une CI/CD GitHub Actions pour l'automatisation des tests et de la documentation.
- **Tech** : SQL, dbt Core, GitHub Actions. Construit avec DuckDB pour le développement local ; architecture pensée pour être portée vers des entrepôts cloud (BigQuery, Snowflake).
- **Impact** : marts prêts pour la BI livrés pour l'analyse de revenu et de rétention. Source de vérité unique établie, avec contrôle qualité automatisé.

---

#### 3. [Prédiction de churn client - Telco](https://github.com/SimonNC/telco-customer-churn-prediction)

> **Outil d'aide à la décision ML : 0.84 ROC-AUC, 0.73 de recall sur les churners.**

```
 7 043 clients
      │
 EDA orientée métier ──► Facteurs clés de churn identifiés
      │
 Pipeline ML sans fuite de données (recall-first)
      │
 Application Streamlit ──► Simulation de stratégies de rétention en temps réel
```

- **Contexte** : le churn client est un risque financier majeur dans le secteur telco - le coût d'acquisition dépasse largement le coût de rétention.
- **Ce que j'ai fait** : conduit une EDA orientée métier sur 7 043 clients pour identifier les facteurs clés de churn. Construit un pipeline ML sans fuite de données avec une stratégie recall-first. Déployé une application Streamlit pour simuler des profils clients et ajuster le seuil de décision.
- **Tech** : Python (Pandas, Scikit-learn), Random Forest, Logistic Regression, Streamlit, Git/GitHub.
- **Impact** : outil actionnable permettant aux équipes métier d'identifier tôt les clients à risque et de simuler des stratégies de rétention à partir de probabilités de churn en temps réel.

---

### 📜 Certifications

| Certification | Statut |
|---|---|
| [Microsoft PL-300 - Power BI Data Analyst Associate](https://learn.microsoft.com/en-us/users/simonjorite-4846/credentials/b2cc3310a92a9302) | Certifié (2025) - [Vérifier le certificat](https://learn.microsoft.com/en-us/users/simonjorite-4846/credentials/b2cc3310a92a9302) |
| Le Wagon - Data Analytics Bootcamp (RNCP niveau 6) | Certifié (2025) |
| AWS Solutions Architect - Associate | En cours |
---

### 🌍 Langues

- **Français** : langue maternelle
- **Anglais** : courant - 6+ ans en environnement anglophone (Dublin, Malte)
- **Espagnol** : conversationnel

---

### 📫 Contact & Opportunités

- **LinkedIn** : [linkedin.com/in/simonjorite](https://www.linkedin.com/in/simonjorite)
- **Email** : simon.jorite@gmail.com
- **Prise de RDV** : [Réserver un échange de 30 min](https://calendly.com/simon-jorite/echange-da)
- **Localisation** : Lyon, France - Ouvert à un poste hybride ou en télétravail

*Data Analyst certifié PL-300, double culture data et finance. Disponible sur Lyon et périphérie - CDI, CDD ou missions freelance.*
