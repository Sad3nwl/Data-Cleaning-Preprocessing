# World Happiness Report 2015 - Data Analysis Pipeline

This repository contains a Python-based exploratory data analysis (EDA) pipeline that analyzes the global happiness scores and rankings from the World Happiness Report 2015. The project focuses on statistical exploration, correlation analysis, and custom data binning to extract meaningful socio-economic insights.

---

## 📌 Project Objectives & Insights

The analysis systematically evaluates 158 countries across 12 statistical features to answer key exploratory questions:

### 1. Extremes in Global Happiness
* **Top 2 Happiest Countries:** Switzerland ($7.587$) and Iceland ($7.561$).
* **Bottom 2 Happiest Countries:** Togo ($2.839$) and Burundi ($2.905$).

### 2. Regional Excellence
* Aggregated data by geographic regions to find out that **Australia and New Zealand** holds the highest average happiness score globally.

### 3. Key Driving Factors
* Conducted a Pearson correlation analysis across all numeric factors (GDP, Family, Health, Freedom, Trust, Generosity).
* **Insight:** `Economy (GDP per Capita)` emerged as the single factor most strongly associated and correlated with a higher overall Happiness Score.

### 4. Custom Feature Engineering (`HAPPINESS_LEVEL`)
Engineered a new categorical feature to group global happiness levels based on threshold conditions:
* 🟢 **High:** $\text{Score} \ge 7$ (15 countries)
* 🟡 **Medium:** $5 \le \text{Score} < 7$ (78 countries)
* 🔴 **Low:** $\text{Score} < 5$ (65 countries)

---

## 📊 Dataset Structure
The analysis processes `happines2015.csv` containing 158 non-null records with features including:
* `Country` & `Region` (Categorical)
* `Happiness Rank` & `Happiness Score` (Target Metrics)
* Socio-economic factors: `Economy (GDP per Capita)`, `Family`, `Health (Life Expectancy)`, `Freedom`, `Trust (Government Corruption)`, `Generosity`.

---

## 🚀 How to Run the Project

### Prerequisites
Ensure you have the required data manipulation and visualization packages installed:
```bash
pip install pandas matplotlib seaborn
### MADE by :
sadeen abdelalrahman
