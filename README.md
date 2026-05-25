#  Alternative Credit Scoring Pipeline for the Creative Economy
An end-to-end Machine Learning and Business Intelligence solution designed to assess credit risk for digital creators using alternative data footprints.

##  Business Case & Context
Traditional banking credit models rely heavily on formal payslips and collateral, completely locking out the booming **Creative Economy**. This project builds an alternative credit scoring pipeline tailored for financial institutions (like Equity Bank) to safely tap into this multi-billion shilling market while protecting asset quality and mitigating Non-Performing Loans (NPLs).

By leveraging alternative data—such as **production consistency** and **audience traffic growth**—this pipeline automates risk assessment and segments applicants into actionable operational tiers.

---

##  Project Architecture & Pipeline
The project is split into two distinct, production-ready layers:

### 1.  Backend Machine Learning Pipeline (`01_alternative_credit_scoring_model.ipynb`)
* **Data Synthesis:** Developed a custom Python data generation engine simulating realistic digital footprints for 251 content creators across various niches (Digital Video, Music, Fashion, Fine Art).
* **Feature Engineering:** Quantified creator risk profiles using novel metrics: `upload_consistency_index`, `view_growth_rate_90d`, and `audience_sentiment_score`.
* **Predictive Modeling:** Trained a **Decision Tree Classifier** baseline model (Achieved **64.7% validation accuracy**).
* **Risk Tiering Logic:** Transformed continuous probability weights into three operational business buckets: `Low Risk (Fast-Track)`, `Medium Risk (Review)`, and `High Risk (Reject)`.

### 2.  Frontend Executive Dashboard (`02_alternative_credit_scoring_dashboard.pbix`)
* Ingested the ML-scored pipeline output into **Power BI**.
* Engineered custom **DAX Measures** to compute key banking metrics dynamically:
  * `Total Applications` (Portfolio size tracking)
  * `Total Exposure KES` (Aggregated capital at risk)
  * `Average Default Probability` (Real-time portfolio health monitoring)
* Implemented cross-filtering visuals allowing credit risk managers to segment risk profile distributions by creative niche instantly.

---

## Tech Stack
* **Languages:** Python (Pandas, NumPy, Scikit-Learn)
* **Business Intelligence:** Power BI, DAX
* **Environment:** Jupyter Notebook

---

##  Operational Impact & Key Findings
* **Portfolio Overview:** Processed 251 applications representing **57.50M KES** in total requested loan exposure.
* **Risk Concentration:** The model safely flagged **25.5%** of applicants as high-risk anomalies, saving the bank from potentially severe NPL exposure.
* **Automated Efficiency:** Identified **20.32%** of applicants as low-risk candidates eligible for automated mobile disbursement (e.g., instant digital lending integration).

*Developed by Ashley 
