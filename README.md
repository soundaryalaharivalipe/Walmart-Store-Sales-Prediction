#Walmart Store Sales Prediction
## Project Overview

This project aims to develop machine learning models to predict weekly sales for various departments across different Walmart stores. Accurate sales forecasting helps Walmart in business planning, budgeting, and organizing promotional events efficiently.

## Project Description

## Background
Walmart operates numerous stores across the country, and accurate sales forecasts are critical for managing inventory, staffing, and promotional events. This project uses data from the Kaggle "Walmart Recruiting - Store Sales Forecasting" competition to predict sales for various departments in Walmart stores.

## Problem Statement
Sales predictions are affected by holidays, markdown events, and other factors. Our goal is to build a machine learning model that can predict future sales considering these factors, providing Walmart with actionable insights.

## Data Description
The data consists of historical sales data for 45 Walmart stores, including:
- **store.csv:** Detailed information about the stores.
- **train.csv:** Historical sales data.
- **test.csv:** Test data for predictions.
- **features.csv:** Additional data like fuel price, temperature, and markdown events.

## Methodology

Data Preprocessing
- **Missing Values:** Filled missing values in Markdown fields with 0 and used mean values for CPI and Unemployment.
- **Encoding Categorical Data:** Converted categorical data in IsHoliday and Type fields to numerical values.
- **Feature Engineering**
  **Holiday Features:** Created features such as Days_to_Thanksgiving, Days_to_Christmas, and indicators for holidays.
  **Markdown Features:** Combined markdown fields into a single MarkdownsSum feature.
- E**xploratory Data Analysis (EDA)** : Analyzed the impact of store type, holidays, store size, and department on weekly sales using visualizations.

## Machine Learning Models
Trained various models including:

- Linear Regression
- Ridge Regression
- Decision Tree
- Random Forest
- Extra Trees
- Model Evaluation

Used **Weighted Mean Absolute Error (WMAE)** as the evaluation metric. Random Forest and Extra Trees models performed best, with Random Forest achieving the lowest WMAE.

**Hyperparameter Tuning**
Optimized parameters for the Random Forest model to improve performance.

## Results

Random Forest and Extra Trees models were the best performers, with Random Forest achieving a WMAE of 1348.38 on the validation dataset. The final submission blended predictions from both models, achieving a top 5% score in the Kaggle competition.

## Conclusion

This project demonstrates the effectiveness of machine learning in predicting store sales, providing valuable insights for inventory management and promotional planning at Walmart.

## Future Work

Implementing deep learning models can further enhance prediction accuracy.


