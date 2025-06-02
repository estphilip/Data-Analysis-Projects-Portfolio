#  Fashion Stock Flow & Trends Dashboard

A data-driven analysis of fashion inventory and sales patterns to help retail businesses reduce stockouts, avoid overstocking, and make smarter discounting decisions  built as part of the #30DaysOfDataWithAnnie challenge.

## Table of Contents

## 1. [Project Overview](#1-project-overview)
## 2. [Data Source](#2-data-source)
## 3. [Key Metrics Tracked](#3-key-metrics-tracked)
## 4. [Tools Used](#4-tools-used)
## 5. [Data Cleaning & Preparation](#5-data-cleaning--preparation)
## 6. [Exploratory Data Analysis](#6-exploratory-data-analysis)
## 7. [Data Analysis (Stats)](#7-data-analysis-stats)
## 8. [Results & Key Findings](#8-results--key-findings)
## 9. [Recommendations & Limitations](#9-recommendations--limitations)
## 10. [References](#10-references)
- [Final Thoughts](#final-thoughts)

---

## 1.  Project Overview

This project analyzes over 15,000 records from an Indian fashion retail dataset to solve a real-world retail problem: how to ensure high-demand products stay in stock while avoiding excess stock of low-demand items.

### Business Problem:

 Stockouts of popular items leading to lost revenue.
 Overstocked items causing waste and poor storage usage.
 Unclear impact of pricing and discounts trends on different customer demographics.

---

## 2.  Data Source

The dataset consists of 15,000+ product-level entries from an Indian fashion retailer, including attributes like product type, color, material, pricing, and sales demographics (men, women, boys, girls,).

---

## 3. 📊 Key Metrics Tracked

- 📦 Stock Flag (In Stock = 1, Out of Stock = 0, Unknown = -1)
- 💰 Discount & Discount %
- 🧍‍♀️ Demographic Target (Men, Women, Boys, Girls and Unisex wears)
- 🧵 Dominant Material & Color
- 📈 Variant Price & Compare-at Price                                                     
- Product Type & Brand Demand Trends
    

---

## 4.  Tools Used

 
 - Excel - Initial cleaning, exploratory analysis
 - Power BI - Dashboard development, DAX logic, data modeling
 - Python (Pandas)- Statistical analysis (correlation, regression, ANOVA)

---

## 5.  Data Cleaning & Preparation

A 9-step approach was applied to ensure clean, analysis-ready data:

1. Unified date formatting (fixed slashes/dashes)
2. Removed Excel color formatting
3. Filled missing values with descriptive placeholders:

    “Unknown Color”
    “Unknown Material”
    “Others” for vague product types
4. Split mixed-size column into text size and numeric size
5. Merged Date and Time into a `DateTime` column
6. Cleaned all text fields (trimmed, capitalized, removed symbols)
7. Created new columns:

    `Discount`, `Discount %`
    `Stock Flag`
8. Removed duplicates using the `ID` column
9. Validated changes before analysis and visualization

---

## 6.  Exploratory Data Analysis [EDA](https://docs.google.com/document/d/1cb65roWMMQTtG-C_zpuJkPO6bwJiw_hlqvVwJfZ_MMU/edit?usp=sharing) 👈

 Visualized stock status across brands, product types, and demographics
 Identified top-selling and slow-moving items
 Assessed discounting patterns by target groups (e.g., women’s seasonal spikes)
 Analyzed color and material popularity

---

## 7. 📈 Data Analysis (Stats)

 Correlation Analysis: Strong positive correlation (r ≈ 0.77) between discount and price
 Linear Regression:

   Each unit increase in discount raised the compare-at price by \~1.22 units (p < 0.001)
 ANOVA & Residuals:

   Demographics had varying sensitivity to discounts
   Weak correlation between discount and stock status (\~0.02), suggesting other influential factors

---

## 8. ✅ Results & Key Findings

 - Items with large discounts tend to be high-priced, not necessarily fast-selling.
 - Discounts do not guarantee stock clearance segment-based strategies are more effective.
 - Stock Flag and Discount are not significantly correlated popular items may sell out regardless of markdown.
 - Women’s products show seasonal spikes (especially August–September), driven by discount events.

---

## 9. 💡 Recommendations & Limitations

### Recommendations:

 - Use targeted discount strategies based on product type and demographic.
- Prioritize stock for trending product types like Straight Kurtas.
 - Incorporate demographic-based forecasting to plan seasonal inventory.

### Limitations:

 - No direct sales quantity data—focused on price and stock availability
 - Data quality varied in some fields (filled with “Unknown” placeholders)
 - Limited time window for demand trend forecasting

---

## 10. 📚 References

 Original dataset (proprietary/simulated retail data for analysis purpose)
 \#30DaysOfDataWithAnnie Challenge Community
 Power BI Documentation
 Pandas & Scikit-learn Documentation

---

##  Final Thoughts

This project showcases how data analysis, when paired with clear business questions, can drive real value in retail decision-making. Whether you're a fashion startup or a large retail chain, understanding stock behavior and discount impacts can save costs and boost customer satisfaction.
# THANK YOU
