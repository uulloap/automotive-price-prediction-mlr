# Automotive Pricing: Multiple Linear Regression & Feature Analysis

![R](https://img.shields.io/badge/Language-R-blue.svg)
![Topic](https://img.shields.io/badge/Domain-Automotive_/_Business-green.svg)
![Method](https://img.shields.io/badge/Method-Multiple_Linear_Regression-orange.svg)

## 📌 Project Overview
This project explores the physical and mechanical attributes that drive vehicle market prices. Using the UCI Automobile dataset, I developed a predictive model that identifies which features—ranging from engine size to body style—most significantly impact a car's valuation.

## 📊 Business Problem
Pricing a vehicle correctly requires balancing technical specifications with market positioning. This analysis provides a data-driven framework for automotive manufacturers and retailers to quantify the "dollar value" of specific upgrades and design choices.



## 🛠️ Technical Stack
- **Language:** R
- **Libraries:** `tidyverse`, `ggplot2`, `readr`, `car`
- **Models:** Multiple Linear Regression (MLR) using Ordinary Least Squares (OLS)
- **Validation:** Residual Analysis, Cook’s Distance, Q-Q Plots, Coefficient of Variation (CV)

## 🚀 Key Features
- **Statistically Robust Model:** Achieved a **Multiple R-squared of 0.9246**, explaining 92.5% of the variance in price across 205 records.
- **Categorical Encoding:** Transformed qualitative data (Fuel Type, Body Style, Engine Location) into dummy variables for inclusion in the regression matrix.
- **Feature Interpretation:** Quantified the financial impact of key variables, such as the **$568 price increase per inch of vehicle width** and the **$7,521 premium** for rear-engine placement.
- **Outlier & Influence Detection:** Utilized **Cook’s Distance** to identify and evaluate influential observations that could bias the pricing model.



## 📈 Key Insights & Results
- **Primary Drivers:** Engine Size ($58.05 per cc) and Curb Weight ($3.91 per lb) were identified as the most consistent positive predictors of price.
- **Model Stability:** The Residual Standard Error (RSE) of **$2,410** provides a clear confidence interval for price predictions on new inventory.
- **Negative Predictors:** Certain body styles and lower cylinder counts were statistically linked to lower price points, allowing for clear market segmentation.

## 📂 Project Structure
```text
├── data/               # UCI Automobile dataset (imports-85.data)
├── notebooks/          # .Rmd file with full data cleaning and OLS logic
├── output/             # Residual plots, Q-Q plots, and feature correlation maps
├── Final_Report.pdf    # Comprehensive business report and model interpretation
└── README.md           # Project documentation
