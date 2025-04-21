# 📊 Page Engagement A/B Testing

This project analyzes user engagement across two landing pages (Page A vs. Page B) using time-on-page as a **proxy metric** for effectiveness. It applies a complete A/B testing workflow, including statistical testing, confidence intervals, bootstrapping, and power analysis. Results are presented in a Jupyter notebook.
---

## 🧪 Project Objective

To determine whether **Page B** leads to higher user engagement (measured by time spent) compared to **Page A**, and provide statistically grounded business recommendations for optimization.

---

## 📈 Features

- Cleaned and explored real-world A/B testing dataset
- Performed **Welch’s t-test** for unequal variances
- Calculated **confidence intervals** (parametric and bootstrap)
- Measured **effect size** (Cohen’s d)
- Conducted **statistical power analysis**
- Visualized time distributions and mean comparisons
- Analysis summary

---

## 🛠 Technologies Used

- **Python** (pandas, numpy, scipy, statsmodels)
- **Visualization**: matplotlib, seaborn, plotly
- **Statistical Testing**: Welch’s t-test, bootstrapping, Cohen’s d
- **Power Analysis**: TTestIndPower (statsmodels)
- **Notebook**: Jupyter

---

## 🚀 How to Run

### ▶ Run Notebook
```bash
jupyter notebook notebook/ab_testing_analysis.ipynb
```

---

## 📊 Dataset Overview

- Sourced from *Practical Statistics for Data Scientists*
- 36 total web sessions:
  - 21 on Page A
  - 15 on Page B
- Engagement measured by time-on-page (in hundredths of a second)

[Dataset on Kaggle](https://www.kaggle.com/datasets/feeldidaxie/landing-page-ab-testing-dataset)

---

## 📌 Key Results

- 📈 **Page B** showed a **28.6% higher** average time (1.62 vs. 1.26 mins)
- ❌ Not statistically significant (p = 0.2815, power = 0.19)
- ✅ Practical effect observed (Cohen’s d = 0.38)
- 📊 Confidence Intervals and Bootstrap CI indicate potential value, but further testing is recommended

---

## 🔍 Next Steps

- Collect more data to increase statistical power
- Extend test to include conversion or click-through metrics
- Make dashboard CSV-upload ready for broader use

---

## 📬 Contact

Created by **Jean-Emmanuel Kouadio**  
