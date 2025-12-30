# 📊 A/B Testing Analysis: Ad vs PSA Conversion

## 🔍 Project Overview
This project analyzes an **A/B testing experiment** to evaluate whether showing
**advertisements (Ads)** leads to higher user conversion compared to showing a
**Public Service Announcement (PSA)**.

The analysis is conducted using Python in **Google Colab** and focuses on
**business-oriented interpretation** of statistical results, making it relevant
for Business Analysts, Product Analysts, Marketing Analysts, and Data Scientists.

---

## 🎯 Business Problem
> Should the company continue investing in advertisements, and how can ad delivery
> be optimized to maximize user conversions?

Advertising budgets are limited, and even small improvements in conversion rates
can lead to significant revenue impact at scale. This project uses experimentation
to reduce decision-making risk.

---

## 📁 Dataset Description
The dataset contains **user-level experimental data**, including:
- **Test Group**: Ad or PSA
- **Converted**: Binary indicator (1 = converted, 0 = not converted)
- **Most Ads Day**: Day of the week with highest ad exposure
- **Most Ads Hour**: Hour of the day with highest ad exposure

Each row represents a **unique user** participating in the experiment.

---

## 🧪 Methodology
The analysis follows a structured A/B testing workflow:

1. Data cleaning and validation
2. Exploratory Data Analysis (EDA)
3. Conversion rate calculation (expressed as percentages)
4. Statistical testing:
   - Chi-squared tests for group comparison
   - Chi-squared tests for day and hour effects
   - Normality and variance checks to validate test selection
5. Business-focused interpretation of results

---

## 📊 Key Results
| Metric | Value |
|------|------|
| Ad conversion rate | **2.55%** |
| PSA conversion rate | **1.79%** |
| Absolute lift | **0.76 percentage points** |
| Relative lift | **~42%** |
| Statistical significance | **Yes (p ≪ 0.05)** |

---

## 🧠 Statistical Reasoning
- Conversion is a **binary outcome**, so normality assumptions do not hold
- Normality (Shapiro–Wilk) and variance (Levene’s) tests confirm that
  **parametric tests are inappropriate**
- **Chi-squared tests** are the correct and reliable statistical approach for
  evaluating differences in conversion behavior

---

## 💼 Business Insights
- Advertisements **significantly outperform** public service announcements in
  driving conversions
- Conversion behavior varies significantly by **day** and **hour** of exposure
- Advertising effectiveness is **not uniform across time**

These insights indicate that **when** ads are shown is as important as **whether**
they are shown.

---

## ✅ Final Recommendation
- Continue using advertisements as a conversion driver
- Optimize ad delivery by focusing on **high-performing days and hours**
- Incorporate advertising cost data in future analysis to evaluate **ROI**

---

## ⚠️ Assumptions & Limitations
- Users are assumed to be randomly assigned to test groups
- Advertising cost and long-term user effects are not included
- Results may not generalize beyond the observed dataset

---

## 🚀 Future Improvements
- Confidence intervals for conversion lift
- ROI and cost-benefit analysis
- Multivariate experimentation
- User segmentation analysis

---

## 🛠️ Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib
- SciPy
- Google Colab / Jupyter Notebook

---

## 📌 Skills Demonstrated
- A/B Testing & Experimentation
- Statistical Analysis
- Business Analytics
- Data-Driven Decision Making
- Analytical Storytelling

---


## ⭐ Summary
This project demonstrates how A/B testing can be used to evaluate marketing
effectiveness, validate decisions with statistical rigor, and translate data
insights into actionable business recommendations.
