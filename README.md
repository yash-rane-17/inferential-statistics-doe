# Inferential Statistics & Design of Experiments (DoE) 📊⚙️

## 📌 Project Overview
This project applies statistical modeling and hypothesis testing frameworks to analyze multi-variable datasets from real world engineering, industrial manufacturing domains. The goal is to substitute intuition with data driven confidence thresholds to solve operational bottlenecks, structural quality control failures and process optimization challenges.

---

## 📂 Business Case Studies & Technical Implementation

### 📦 Case 1: Supply Chain Pilferage & Material Tearing (Normal Distribution)
* **Objective:** Audit the breaking strength of industrial cement packaging bags ($\mu = 5\text{ kg/cm}^2$, $\sigma = 1.5$) to predict supply chain wastage.
* **Methodology:** Utilized Standard Normal Variable ($Z$-score) mapping and `scipy.stats.norm.cdf` to compute critical operational probabilities.
* **Core Insights:**
  * **11.12%** of incoming bags fall below the critical structural threshold of $3.17\text{ kg/cm}^2$, posing a major risk for material tearing.
  * **82.47%** of inventory comfortably meets or exceeds a baseline capacity of $3.6\text{ kg/cm}^2$.
  * Only **13.90%** of inventory heavily deviates from standard quality targets (falling outside the $3.0 - 7.5\text{ kg/cm}^2$ window).

### 🪨 Case 2: Manufacturing Quality Validation (Parametric Hypothesis Testing)
* **Objective:** Verify if unpolished raw stock meets the minimum Brinell Hardness Index of 150 required for optimal pattern printing.
* **Methodology:** Executed a left tailed **One-Sample t-test** ($\alpha = 0.05$) on unpolished data, followed by an independent **Two-Sample t-test** to track post-treatment changes.
* **Core Insights:**
  * The One-Sample test yielded a $p\text{-value} = 4.17 \times 10^{-5}$ ($p \ll 0.05$), statistically confirming that raw unpolished stones are highly unsuitable for production.

### 🦷 Case 3: Process Optimization via Design of Experiments (Factorial ANOVA)
* **Objective:** Evaluate how material hardness varies when multiple factors Treatment Method, Alloy Selection, and Operators interact simultaneously.
* **Methodology:** Implemented a **Three-Way ANOVA / Multi-Factor Analysis of Variance** using `statsmodels.formula.api.ols` to isolate main effects and interaction terms.
* **Core Insights:**
  * Individual human operators did not induce statistically significant variation ($p > 0.05$), proving consistency across handlers.
  * The **Treatment Method** is the single highest driver of material hardness ($p < 0.05$).
  * A significant **Interaction Effect ($Dentist \times Method$)** exists, proving that certain advanced methods require specific pairing matrices to reach maximum structural resilience.

---

## 🛠️ Tech Stack & Libraries Used
* **Language:** Python
* **Statistical Compute:** `scipy.stats`, `statsmodels`
* **Data Engineering:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`

---

## 🤝 Connect with Me
* **LinkedIn:** https://www.linkedin.com/in/yash-rane-275867156/
* **Portfolio Main Page:** https://github.com/yash-rane-17
