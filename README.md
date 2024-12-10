# Retail-Price-Optimization

### Overview

This project focuses on building a predictive model for retail price optimization. The goal is to determine optimal product prices that balance customer demand and maximize revenue, using historical retail data.

Price optimization is crucial for maintaining profitability while keeping customers engaged. By understanding demand patterns and price elasticity, businesses can set competitive prices to achieve their goals.

### Objectives

##### Exploratory Data Analysis (EDA):
- Analyze the distribution of demand, prices, and other features.
- Understand relationships between features using correlation matrices and visualizations.

##### Demand Forecasting:
- Use historical sales data to predict future demand using models like Random Forest and Prophet.

##### Price Optimization:
- Build a Random Forest Regressor to simulate demand for different price points.
- Identify the price that maximizes revenue using predicted demand.

### Dataset

Source: Retail Price Optimization Dataset

Features:
- Product details: product_id, product_category_name, unit_price, etc.
- Demand data: qty (demand quantity).
- Competition data: comp_1, comp_2, comp_3.
- Time features: month_year, weekday, holiday, etc.

### Results

##### MAPE: ~2.39%
- The low MAPE indicates the model is generally accurate relative to the scale of the demand.
- The model performs reasonably well for practical use, especially if the focus is on percentage accuracy (e.g., for pricing decisions).

##### R² Score: 0.32
- The low R² score indicates the model fails to explain a significant portion of the variance in demand, suggesting missing features or non-linear relationships not captured by the model.
- The MAE of 10.14 units suggests there is room to improve the precision of individual predictions.

### Source

https://www.kaggle.com/datasets/suddharshan/retail-price-optimization
