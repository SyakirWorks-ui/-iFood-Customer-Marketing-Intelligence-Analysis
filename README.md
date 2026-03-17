# 🛒 iFood Customer & Marketing Intelligence Analysis
> **End-to-End Data Science Project: From Exploratory Analysis to Predictive Insights**

## 📌 Project Overview
This project analyzes the iFood marketing dataset to uncover customer purchasing patterns, evaluate marketing campaign effectiveness, and identify key drivers of revenue. By leveraging **Exploratory Data Analysis (EDA)**, **Statistical Testing**, and **Predictive Modeling**, this analysis provides actionable recommendations to optimize Marketing ROI and customer retention.

---

## 🎯 Learning Agenda & Business Questions
Based on the project roadmap, the analysis focuses on answering 7 critical business questions:
1. **Customer Profiling**: What are the characteristics of high-value customers?
2. **Spending Patterns**: How does household composition (kids/teens) affect spending?
3. **Marital & Education Impact**: Do demographics influence purchasing power?
4. **Channel Performance**: Which channels drive the most conversions?
5. **Campaign ROI**: How do customers respond to different marketing touches?
6. **Product Affinity**: Which product categories are the primary revenue drivers?
7. **Predictive Modeling**: What factors significantly predict campaign acceptance?

---

## 🚀 Key Insights & Storytelling

### 1. KPI & Business Health Overview
We established a baseline for business performance, focusing on conversion rates and average order values.
![KPI Performance](1.%20Kpi%20ifood.png)
* **Strategic Insight**: Understanding the baseline conversion helps in setting realistic growth targets for future quarters.*

### 2. Customer Segmentation & Spending
Analysis of income vs. spending reveals clear clusters of high-value patrons.
![Customer Segmentation](2a.customer%20segmentation.png)
* **Finding**: Income is the strongest predictor of total spending, but household size plays a crucial moderating role.*

### 3. Revenue Drivers (Linear Regression Results)
Using Multiple Linear Regression, we identified the key variables driving `MntTotal`.
* **Positive Drivers**: `Income`, `NumWebVisitsMonth`.
* **Negative Drivers**: `Kidhome` (Significantly reduces spending in premium categories).
![Product Analysis](6a.%20product%20%20&%20inventory.png)

### 4. Predictive Targeting (Logistic Regression)
To optimize marketing spend, a Logistic Regression model was built to predict the probability of a customer accepting a campaign.
![Marketing Performance](5.%20marketing%20&%20channel%20performance.png)
* **Key Result**: Customers with lower `Recency` (recent shoppers) and higher `Income` are **70.3% more likely** to respond to promotions (Odds Ratio: 1.70).*

### 5. Retention & Churn Risk
By analyzing `Recency` and engagement, we identified segments at risk of churning.
![Churn Risk](3.%20churn%20risk.png)
* **Recommendation**: Implement a re-engagement campaign for customers who haven't purchased in >60 days.*

---

## 🛠️ Tech Stack & Methodology
* **Language**: Python 3.x
* **Libraries**: Pandas, NumPy, Scipy (Statistics)
* **Modeling**: Statsmodels (OLS & Logit Regression)
* **Visualization**: Seaborn, Matplotlib
* **Workflow**:
    * **Stage 01**: Data Cleaning & EDA
    * **Stage 02**: Statistical Hypothesis Testing & Regression
    * **Stage 03**: Strategic Insight Communication

---

## 📂 Project Structure
```text
├── data/
│   ├── raw/                # Original ifood_df.csv
│   └── processed/          # Cleaned dataset for modeling
├── notebooks/
│   ├── 01_eda_understanding.ipynb
│   ├── 02_statistical_analysis.ipynb
│   └── 03_visualization_insight.ipynb
├── outputs/
│   ├── figures/            # Exported plots and charts
│   ├── reports/            # Automated statistical summaries (.txt)
│   └── tables/             # Regression coefficient tables (.csv)
└── README.md

---
```


## 📈 Final Recommendations & Business Impact

Based on the multi-stage analysis and predictive modeling, the following strategic actions are recommended to optimize iFood's marketing performance:

### 1. High-Value Segment Prioritization
* **Strategy**: Allocate **60% of the marketing budget** to the "High-Income, No-Child" segment.
* **Rationale**: Analysis confirms this group has the highest `MntTotal` and lowest price sensitivity.
* **Action**: Create premium "Child-Free Weekend" bundles featuring 'Wine' and 'Meat' products.

### 2. Campaign Response Optimization
* **Strategy**: Implement a **"Recency-Triggered"** automated mailing system.
* **Rationale**: Logistic Regression results show that customers who purchased within the last 30 days are **70.3% more likely** to accept a new offer (Odds Ratio: 1.70).
* **Action**: Send a follow-up promotion exactly 7 days after a successful transaction to capitalize on engagement momentum.

### 3. Web Channel Conversion Boost
* **Strategy**: Gamify web visits to increase monthly frequency.
* **Rationale**: `NumWebVisitsMonth` is a significant positive driver of total revenue.
* **Action**: Offer "Web-Only" flash sales to transition offline-heavy shoppers to the digital ecosystem where tracking and retargeting are more effective.

### 4. Churn Mitigation & Win-Back
* **Strategy**: Deploy an automated win-back campaign for customers crossing the **60-day inactivity threshold**.
* **Rationale**: Visual analysis of `Recency` shows a sharp decline in response probability after 2 months of inactivity.
* **Action**: Provide a "We Miss You" 20% discount specifically for their most-purchased category (e.g., Gold products or Sweets).

---

## 👨‍💻 Technical Appendix & Reproducibility
To replicate this analysis, ensure you have the environment set up as follows:

1.  **Clone the Repository**:
    ```bash
    git clone [https://github.com/username/ifood-marketing-analysis.git](https://github.com/username/ifood-marketing-analysis.git)
    ```
2.  **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run Pipeline**: Execute notebooks in order: `01_EDA` -> `02_Statistical_Analysis` -> `03_Visualization`.

---

## 🤝 Contact & Contribution
I am a Data Analyst passionate about transforming complex datasets into clear business narratives. Feel free to reach out for collaboration or inquiries!

* **Author**: [Muhamad Syakirullah]
* **LinkedIn**: [https://www.linkedin.com/in/syakirworks/]
* **Email**: [syakirworksid@gmail.com]
* **Fiverr**: [https://www.fiverr.com/sellers/tajulmuluk/]

---
*Developed as part of the iFood Marketing Intelligence Project - 2026*
