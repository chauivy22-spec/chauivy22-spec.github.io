---
permalink: /projects/
title: "Project"
author_profile: true
---
## Project 3: Energy Sector M&A — Predicting Shareholder Value

Built a logistic regression classification model on 56 U.S. energy-sector M&A deals (2005–2024), using pre-deal financial data collected from the SEC EDGAR XBRL API to predict whether acquisitions create or destroy shareholder value. Applied the model to four unseen Houston-area acquisitions as a real-world case study.

#### Key Insights

- Engineered pre-deal financial features including **ROA, D/E ratio, EPS, and deal value** from SEC 10-Q/10-K filings using the XBRL `companyfacts` API.
- Used **median imputation** to reduce the impact of extreme financial outliers.
- Found that higher **D/E ratio and EPS** were associated with higher odds of value creation, while larger deal size was associated with lower odds.
- Achieved a cross-validated **AUC-ROC of 0.522**, demonstrating that four financial features alone provide limited predictive power for M&A outcomes.
- Applied the model to four real, unseen **Houston-area acquisitions**, all classified as value-destroying, with ExxonMobil–Pioneer receiving the lowest predicted probability of value creation at **5.5%**.
- Identified key limitations including **small sample size, limited financial variables, and lack of macroeconomic/post-deal factors**, and proposed expanded datasets and tree-based models for future analysis.

#### Tools

- Python (scikit-learn, pandas)
- SEC EDGAR XBRL API
- Data Collection & Feature Engineering
- Logistic Regression
- Financial Ratio Analysis
- Cross-Validation & Model Evaluation (ROC-AUC, Confusion Matrix, Classification Report)

## Project 2: Bank Marketing Campaign — Term Deposit Prediction

Built a leakage-controlled classification pipeline using the UCI Bank Marketing dataset (45,211 customers) to predict term deposit subscriptions and support data-driven marketing targeting. Compared Logistic Regression, Decision Tree, Random Forest, and LightGBM using stratified cross-validation and an ablation study to evaluate real-world deployment feasibility.

#### Key Insights

- Selected **LightGBM as the final model**, achieving **0.9269 test ROC-AUC, 0.8667 recall, and 0.5349 MCC** on a held-out 9,043-customer test set.
- Addressed severe **class imbalance (88.3% vs. 11.7%)** using stratified splitting/CV, class weighting, and ROC-AUC/MCC as primary evaluation metrics.
- Applied a **signed log1p transformation** to reduce skew in heavy-tailed financial features, improving skew from 8.36 to -1.58.
- Conducted an **ablation study showing that `duration` inflates model performance**, with ROC-AUC dropping from 0.9275 to 0.7814 when the post-call feature was removed.
- Identified **`poutcome_success` and contact month** as the strongest legitimate pre-call predictors of subscription likelihood.
- Found that model probabilities were **poorly calibrated**, highlighting the need for Platt scaling or isotonic regression before deployment as risk scores.

#### Tools

- Python (scikit-learn, LightGBM)
- Feature Engineering & Preprocessing Pipelines
- Cross-Validation & Hyperparameter Tuning
- Imbalanced Classification
- Model Evaluation (ROC-AUC, Recall, F1, MCC)
- Ablation Analysis
- Probability Calibration

## Project 1: Game Market Pulse — Visualizing Video Game Sales, Genre Trends, and Critical Reception (1980–2024)

Analyzed ~18,000 video game titles released between 1980–2024 to explore trends in sales, genres, publishers, and critic reception. Built an interactive Tableau dashboard with linked filters to compare market performance across decades.

### Key Insights
- Identified **2005–2010 as a “Golden Age”** of physical game sales during the Wii/PS3/Xbox 360 era.
- Found a significant relationship between **critic scores and sales**, with a 1-point score increase associated with ~340K additional units sold.
- Identified strong **market concentration** among major publishers and genres, with *GTA V* reaching 64.29M units sold.
- Found evidence of a shift toward **fewer, higher-impact blockbuster releases** in the 2010s.
- Highlighted how the transition to **digital distribution** affects the interpretation of historical sales data.

### Tools
- Tableau
- Data Visualization
- Exploratory Data Analysis
- Linear Regression
- Interactive Dashboard Design

