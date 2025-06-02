#  Fashion Stock Flow & Trends Dashboard

  #### A data-driven analysis of fashion inventory and sales patterns to help retail businesses reduce stockouts, avoid overstocking, and make smarter discounting decisions  built as part of the #30DaysOfDataWithAnnie challenge.
#### Dashboard
![Dashboard](https://github.com/user-attachments/assets/538058fd-8f2c-4ffe-af37-1901b5d8f8d9)

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Key Metrics Tracked](#key-metrics-tracked)
- [Tools Used](#tools-used)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis (Stats)](#data-analysis-stats)
- [Results & Key Findings](#results--key-findings)
- [Recommendations & Limitations](#recommendations--limitations)
- [References](#references)
- [Final Thoughts](#final-thoughts)


##   Project Overview

This project analyzes over 15,000 records from an Indian fashion retail dataset to solve a real-world retail problem: how to ensure high-demand products stay in stock while avoiding excess stock of low-demand items.

### Business Problem:

 Stockouts of popular items leading to lost revenue.
 Overstocked items causing waste and poor storage usage.
 Unclear impact of pricing and discounts trends on different customer demographics.

---

## Data Source

The dataset consists of 15,000+ product-level entries from an Indian fashion retailer, including attributes like product type, color, material, pricing, and sales demographics (men, women, boys, girls,).

---

##  Key Metrics Tracked 
- 📦 Stock Flag (In Stock = 1, Out of Stock = 0, Unknown = -1)
- 💰 Discount & Discount %
- 🧍‍♀️ Demographic Target (Men, Women, Boys, Girls and Unisex wears)
- 🧵 Dominant Material & Color
- 📈 Variant Price & Compare-at Price                                                     
- Product Type & Brand Demand Trends
    

---

## Tools Used

 
 - Excel - Initial cleaning, exploratory analysis
 - Power BI - Dashboard development, DAX logic, data modeling
 - Python (Pandas)- Statistical analysis (correlation, regression, ANOVA)

---

## Data Cleaning & Preparation

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

## Exploratory Data Analysis 
[EDA](https://docs.google.com/document/d/1cb65roWMMQTtG-C_zpuJkPO6bwJiw_hlqvVwJfZ_MMU/edit?usp=sharing) 👈

 Visualized stock status across brands, product types, and demographics
 Identified top-selling and slow-moving items
 Assessed discounting patterns by target groups (e.g., women’s seasonal spikes)
 Analyzed color and material popularity

---

## Data Analysis (Stats)

 Correlation Analysis: Strong positive correlation (r ≈ 0.77) between discount and price
 Linear Regression:

   Each unit increase in discount raised the compare-at price by \~1.22 units (p < 0.001)
 ANOVA & Residuals:

   Demographics had varying sensitivity to discounts
   Weak correlation between discount and stock status (\~0.02), suggesting other influential factors

---

##  Results & Key Findings

 - Items with large discounts tend to be high-priced, not necessarily fast-selling.
 - Discounts do not guarantee stock clearance segment-based strategies are more effective.
 - Stock Flag and Discount are not significantly correlated popular items may sell out regardless of markdown.
 - Women’s products show seasonal spikes (especially August–September), driven by discount events.

---

##  Recommendations & Limitations

### Recommendations:

 - Use targeted discount strategies based on product type and demographic.
- Prioritize stock for trending product types like Straight Kurtas.
 - Incorporate demographic-based forecasting to plan seasonal inventory.

### Limitations:

 - No direct sales quantity data—focused on price and stock availability
 - Data quality varied in some fields (filled with “Unknown” placeholders)
 - Limited time window for demand trend forecasting

---

##  References

 Original dataset (proprietary/simulated retail data for analysis purpose)
 \#30DaysOfDataWithAnnie Challenge Community
 Power BI Documentation
 Pandas & Scikit-learn Documentation

---

##  Final Thoughts

This project showcases how data analysis, when paired with clear business questions, can drive real value in retail decision-making. Whether you're a fashion startup or a large retail chain, understanding stock behavior and discount impacts can save costs and boost customer satisfaction.
# THANK YOU
