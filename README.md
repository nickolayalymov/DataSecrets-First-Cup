# 🍕 Dodo Pizza: Promo Response Prediction

<p align="left">
  <img src="https://img.shields.io/badge/ML-Classification-blue.svg" alt="ML">
  <img src="https://img.shields.io/badge/Python-3.10-green.svg" alt="Python">
  <img src="https://img.shields.io/badge/Rank-7th%20Place-gold.svg" alt="Rank">
  <img src="https://img.shields.io/badge/Metric-ROC--AUC%200.7234-orange.svg" alt="Metric">
</p>

## 📌 Project Overview
This repository contains a high-performance solution for the **Data Secrets x Dodo Pizza Hackathon**. The objective was to predict the probability of a customer redeeming a promo code based on multi-source data: order history, mobile app events, and campaign mechanics.

**Key Achievement:** Ranked **7th** out of 75+ participants.

## 🚀 Pipeline Workflow
The project is divided into three logical stages for better reproducibility and transparency:

1.  **Exploratory Data Analysis (EDA):** 
    *   Analyzed customer behavior patterns and promo usage frequency.
    *   Identified key correlations between order types (Delivery vs. Restaurant) and conversion.
    *   Visualized target distribution and handled data imbalance.
2.  **Feature Engineering:**
    *   Generated time-based features from campaign durations.
    *   Created user activity metrics from mobile event logs.
    *   Engineered behavioral features (average check, order frequency, preferred product categories).
3.  **Inference & Submission:**
    *   Optimized model for the 2.0s inference time constraint.
    *   Generated final probability scores for the test dataset.

## 📂 Project Structure
```text
├── data/
│   └── samples/          # Data structure examples (first 5 rows)
├── docs/                 # Detailed documentation
│   ├── img/              # Visual assets
│   ├── competition.md    # Business context
│   ├── task.md           # Technical requirements
│   └── leaderboard.md    # Final standings
├── notebooks/            # Core logic
│   ├── EDA.ipynb         # Data discovery
│   ├── feature_engineering.ipynb
│   └── inference.ipynb   # Final prediction script
├── submit/               # Final predictions (CSV)
└── requirements.txt      # Environment dependencies
```

## 🛠 Tech Stack
*   **Core:** `Python 3.10`, `Pandas`, `NumPy`
*   **ML:** `Scikit-learn`, `CatBoost` / `LightGBM`
*   **Analysis:** `Matplotlib`, `Seaborn`
*   **Environment:** `PyCharm`, `Git`

## 📖 Documentation
For a deep dive into the project details, please visit:
*   <a href="./docs/competition.md" target="_blank">**Competition Overview**</a>
*   <a href="./docs/task.md" target="_blank">**Technical Task**</a>
*   <a href="./docs/leaderboard.md" target="_blank">**Leaderboard Standings**</a>

## 📊 Data Policy
Full datasets are excluded due to licensing restrictions. Data schema and samples are available in the <a href="./data/samples/" target="_blank">`data/samples/`</a> directory.

---
*Developed by <a href="https://github.com/nickalymov" target="_blank">Nick Alymov</a>*
```