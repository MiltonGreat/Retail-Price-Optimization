# Retail-Price-Optimization

### Overview

Price optimization uses historical data to identify the most appropriate price for a product or service that maximizes a company's profitability. Effective pricing considers various factors such as demographics, operating costs, competitive pricing, survey data, and product value. Businesses regularly upgrade their offerings, and pricing must reflect these changes while ensuring competitiveness and sustainability.

### Why is Price Optimization Important?

- Overpricing may lead to customer loss.
- Underpricing reduces revenue and profitability.
- Optimal pricing strikes a balance between business goals and customer satisfaction.

This project implements machine learning models to determine the optimal price by predicting demand and maximizing revenue.

### Dataset

Source: Retail Price Optimization Dataset

Features:
- Product details: product_id, product_category_name, unit_price, etc.
- Demand data: qty (demand quantity).
- Competition data: comp_1, comp_2, comp_3.
- Time features: month_year, weekday, holiday, etc.

### Methodology

1. Data Preprocessing
- Handling missing values and outliers
- Feature engineering and encoding categorical variables
- Creating interaction terms between pricing factors

2. Model Selection & Training
- Used Random Forest, XGBoost, and Gradient Boosting for price-demand prediction
- Tuned hyperparameters using RandomizedSearchCV
- Evaluated models based on MSE, MAE, MAPE, and R²

3. Price Optimization
- Simulated demand by varying price points within a realistic range
- Predicted demand using the best-performing model (XGBoost)
- Maximized revenue by identifying the price that yields the highest revenue

### Visualization

The project includes:

- Feature Importance Analysis (XGBoost feature contributions)
- Residual Plot (Error distribution analysis)
- Revenue vs. Price Plot (To visualize optimal pricing)

### Results

Best Model: XGBoostPerformance Metrics:
- MSE: 1.76
- MAE: 0.65
- MAPE: 0.05
- R²: 0.99

Optimal Price: $1.00 (based on simulated revenue maximization)

### Source

Dataset: [Retail Price Optimization Dataset on Kaggle](https://www.kaggle.com/datasets/suddharshan/retail-price-optimization)
