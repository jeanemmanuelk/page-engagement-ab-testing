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
jupyter notebook ab_testing_analysis.ipynb
```

---

## 📊 Dataset Overview

- Sourced from *Practical Statistics for Data Scientists*
- 36 total web sessions:
  - 21 on Page A
  - 15 on Page B
- Engagement measured by time on page. The raw `Time` values are in units of 100 seconds (the source book's code multiplies them by 100 to get seconds), so Page A averaged about 126 seconds and Page B about 162 seconds. The notebook labels these values as minutes, which is wrong.

[Dataset on Kaggle](https://www.kaggle.com/datasets/feeldidaxie/landing-page-ab-testing-dataset)

---

## 📌 Key Results

- 📈 **Page B** showed a **28.2% higher** average time (1.62 vs. 1.26 in the data's units, about 162 vs. 126 seconds)
- ❌ Not statistically significant (p = 0.2815, power = 0.19)
- 📏 Small-to-moderate effect size (Cohen’s d = 0.38), but the test is underpowered, so this is not yet evidence of a real difference
- 📊 The 95% confidence intervals for the two pages overlap heavily, so the data cannot rule out no difference. More data is needed before acting on this

---

## 🔍 Next Steps

- Collect more data to increase statistical power
- Extend test to include conversion or click-through metrics
- Make dashboard CSV-upload ready for broader use

---

## 📬 Contact

Created by **Jean-Emmanuel Kouadio**  
