# 🍷 Wine Quality - Statistical Exploratory Data Analysis (EDA)

This repository contains a comprehensive Exploratory Data Analysis (EDA) and preprocessing workflow for the **Red Wine Quality** dataset using Python. The analysis focuses on understanding chemical properties, identifying underlying distribution shapes, and preparing data for downstream machine learning tasks.

---

## 📊 Dataset Overview

* **Dataset Size:** 1,599 initial observations across 12 features.
* **Missing Values:** 0 null values across all features.
* **Cleaning:** Deduplication performed to ensure distinct records.

---

## 🔬 Key Statistical Analyses

1. **Variance & Spread Analysis:**
   - Evaluated feature variability; `total sulfur dioxide` ($\sigma^2 \approx 1116.16$) and `free sulfur dioxide` ($\sigma^2 \approx 109.15$) display high variance compared to physicochemical attributes like `pH` and `density`.

2. **Distribution Shapes (Skewness & Kurtosis):**
   - **Leptokurtic (Heavy-Tailed):** `residual sugar` (skewness: 4.55, kurtosis: 28.52) and `chlorides` (skewness: 5.50, kurtosis: 41.58) exhibit severe right-skewness and extreme tail behavior.
   - **Platykurtic (Flatter):** `citric acid` shows flatter distribution metrics (Fisher kurtosis: -0.79).

3. **Outlier Detection:**
   - Isolated multi-variable statistical anomalies using a $Z$-score threshold ($\vert{}Z\vert{} > 3$).

---

## 🛠️ Tech Stack & Libraries

* **Language:** Python 3.x
* **Data Manipulation:** `pandas`, `numpy`
* **Statistical Computing:** `scipy.stats`
* **Visualization:** `seaborn`, `matplotlib`

---

## 🚀 Next Steps

* Feature engineering and scaling.
* Supervised classification modeling (Predicting wine quality ratings).
