# FMCG Global Demand Planning and Forecasting

*A Data Science Capstone Project exploring demand patterns, product segmentation, promotional effects and machine learning-based demand forecasting using three years of FMCG sales data.*

## 1. Project Overview

Demand forecasting is an important aspect of inventory management in the Fast-Moving Consumer Goods (FMCG) industry. Inaccurate forecasts can result in overstocking, increased inventory costs and stockouts, leading to lost sales and reduced customer satisfaction.

This project applies data science techniques to analyse FMCG sales data, identify demand patterns and develop predictive models that can support better inventory planning and decision-making.

## 2. Problem Statement

FMCG businesses operate in dynamic environments characterised by changing consumer demand, promotional activities, price variations and seasonal fluctuations.

The project investigates how historical sales patterns and other business variables can be used to understand demand behaviour and improve daily demand forecasting.

## 3. Project Objectives

- Explore historical FMCG sales patterns and identify demand trends.
- Investigate the relationship between pricing, discounts, promotions and sales volume.
- Segment products using ABC-XYZ analysis.
- Engineer time-series features to capture historical demand patterns.
- Develop and evaluate machine learning models for daily demand forecasting.
- Identify insights that can support inventory planning and supply chain decisions.

## 4. Dataset Description

The project uses three years of FMCG sales data covering January 2021 to December 2023.

Key dataset characteristics:

- 1,100,000 transaction-level observations.
- 102 unique SKUs.
- 7 countries and 9 cities.
- Four sales channels: Hypermarket, Supermarket, E-commerce and Convenience.
- Variables covering sales, pricing, promotions, inventory, geography and logistics.

The original dataset is approximately 212 MB. Large source and cleaned datasets are excluded from GitHub.

## 5. Tools and Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook
- Git and GitHub

## 6. Project Methodology

The project follows a structured data science workflow:

1. Data Exploration and Understanding
2. Data Cleaning and Preparation
3. Exploratory Data Analysis (EDA)
4. ABC-XYZ Product Segmentation
5. Price and Promotion Analysis
6. Time-Series Feature Engineering
7. Demand Forecasting using Linear Regression and Random Forest

## 7. Key Findings

### Exploratory Data Analysis
- Demand varied across months, with higher sales observed between June and August.
- Weekend sales were approximately 19.77% higher than weekday sales on average.
- Beverages recorded the highest total sales volume among the analysed product categories.

### ABC-XYZ Segmentation
- 49 SKUs were classified as A-products, contributing approximately 79.42% of total revenue.
- 29 SKUs were classified as B-products.
- 24 SKUs were classified as C-products.
- XYZ segmentation identified 26 stable, 50 variable and 26 highly variable SKUs.

### Price and Promotion Analysis
- Average sales volume increased across the observed discount levels.
- Products with discounts recorded higher average sales than products without discounts.
- The observed relationships are associative and do not independently establish causation.

### Demand Forecasting

Two regression models were evaluated using a time-based holdout period covering July to December 2023.

| Model | MAE | RMSE | MAPE |
|---|---:|---:|---:|
| Linear Regression | 124.68 | 213.31 | 22.06% |
| Random Forest | 126.95 | 221.06 | 18.35% |

Linear Regression achieved lower MAE and RMSE, while Random Forest achieved a lower MAPE.

Feature importance analysis showed that rolling averages were the most influential predictors in the Random Forest model.

## 8. Ethical Considerations and Limitations

The project considers the implications of forecasting errors for inventory allocation and product availability.

However, the dataset does not contain a Traditional Trade category, limiting the ability to directly assess potential disparities between traditional and modern retail channels.

Other limitations include the observational nature of the dataset, the restricted geographical and product coverage compared with the project guide's illustrative specifications, and the selection of only ten SKUs for forecasting.

Sales observations may also underestimate actual demand during stockout periods.

## 9. Repository Structure

```text
fmcg-demand-forecasting-capstone/
│
├── data/
│   ├── README.md
│   └── fmcg_sales_features.csv
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_data_exploratory_data_analysis.ipynb
│   ├── 04_abc_xyz_segmentation.ipynb
│   ├── 05_price_promotion_analysis.ipynb
│   ├── 06_feature_engineering.ipynb
│   └── 07_demand_forecasting.ipynb
│
├── .gitignore
└── README.md
```

## 10. Conclusion

This project demonstrates how data science and machine learning techniques can be applied to FMCG demand planning.

The findings highlight the importance of historical demand patterns, product segmentation and promotional analysis in understanding sales behaviour.

The forecasting models provide a foundation for more informed inventory planning, although further improvements and validation would be necessary before deployment in a real-world supply chain environment.
