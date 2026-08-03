# ipl-data-analysis
End-to-end IPL analytics pipeline performing multi-season performance analysis, player impact metrics, and match-outcome factors using Pandas and visualization tools.

# 🏏 Indian Premier League (IPL) Data Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/999ssg/ipl-data-analysis/blob/main/Project_IPL_DataAnalysis_Case_Study_SuchismitaSengupta.ipynb)

An end-to-end Exploratory Data Analysis (EDA) and data processing pipeline inspecting historical Indian Premier League (IPL) ball-by-ball and match dataset records to uncover team performance trends, venue impact factors, and individual player impact metrics.

---

## 📌 Situation
Sports analytics relies heavily on extracting actionable insights from granular, high-volume event logs (ball-by-ball data). Franchise managers, analysts, and strategists require clean data pipelines that translate raw match logs into clear performance indicators—such as venue-specific toss advantages, death-over run rates, and high-value player matchups.

---

## 🎯 Task
* Ingest and clean multi-season IPL match and ball-by-ball datasets containing historical match outcomes.
* Perform complex data transformations and aggregations to evaluate team win-rates, venue-specific pitch bias (batting 1st vs. chasing), and toss impact.
* Compute custom player performance metrics (e.g., economy rate in powerplays/death overs, strike rate, boundary frequency).
* Present findings through highly informative, production-ready static and interactive visualizations.

---

## 🛠️ Action & Architecture
1. **Data Cleaning & Pipeline Processing:**
   * Handled missing value imputation for abandoned/rain-affected matches (DLS method records).
   * Standardized team and player names across different seasons to maintain data integrity across franchise rebrandings.

2. **Exploratory Analytics & Feature Engineering:**
   * Calculated **Toss Decision vs. Match Victory** correlations using pivot tables and groupby aggregations.
   * Engineered rolling performance features (e.g., strike rate over last 10 matches) to track player form trends.
   * Derived venue performance profiles analyzing average 1st-innings totals vs. success rate when chasing.

3. **Data Visualization:**
   * Constructed structured plots using `matplotlib` and `seaborn` to highlight top run-scorers, wicket-takers, and head-to-head franchise dynamics.

---

## 📈 Results & Impact
* **Data Integrity:** Built a modular cleaning pipeline converting raw unstructured match logs into structured analytical tables.
* **Key Findings:** 
  * Quantified the statistical impact of toss decisions across specific stadiums (e.g., chasing preference at high-altitude/dew-affected venues).
  * Identified top clutch performers by evaluating strike rates during death overs (overs 16–20).
* **Reproducible Design:** Fully structured workflow built inside Google Colab, allowing for seamless execution and interactive analysis.

---

## 📂 Repository Structure

├── IPL_Data_Analysis.ipynb  # Primary Colab Notebook
├── IPL_Data_Analysis.pdf    # Static PDF Export Report
└── README.md                # Project Overview

---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Data Wrangling:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
