# FUTURE_ML_Task1
https://ai.studio/apps/9efd179c-8014-4729-8516-ace54f099ff3?fullscreenApplet=true

Act as an expert Senior Data Scientist and Full-Stack Machine Learning Engineer. I need to build a complete, production-ready Time-Series Sales Forecasting Application using Python.
The goal is to take historical sales data, clean it, perform time-based feature engineering, train forecasting models, evaluate them, and present the results in a beautiful, business-friendly interactive dashboard using Streamlit and Matplotlib/Seaborn.
Please provide the complete, modular Python code structured into clean scripts or a single cohesive Streamlit application block. Adhere to the following specifications:
1. Data Generation & Ingestion
Create a synthetic but highly realistic historical sales dataset spanning the last 3 years up to the current date.
The dataset should include columns: Date, Product_Category, Sales_USD, and Units_Sold.
Incorporate realistic patterns: a clear upward trend, strong weekly/monthly seasonality (e.g., spikes on weekends and holiday seasons like November/December), and random white noise.
2. Data Cleaning & Feature Engineering
Ensure the Date column is handled correctly as a datetime index.
Engineer time-based features: Year, Month, Day, DayOfWeek, Is_Weekend, and lag features (e.g., Lag_7, Lag_30) or rolling averages to capture historical dependencies.
3. Machine Learning & Forecasting Models
Split the data into training and testing sets using a time-series safe split (do not shuffle).
Implement at least two forecasting approaches for comparison:
A Baseline/Regression approach (e.g., Random Forest Regressor or XGBoost using the engineered time features).
A traditional Statistical/Time-Series approach (e.g., Prophet or a simple Exponential Smoothing/ARIMA if dependencies are light, or a rolling window forecast).
Generate forecasts for the next 30 to 90 days.
4. Model Evaluation & Error Analysis
Calculate and display key business metrics on the test set: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE).
Provide a brief textual interpretation of what these errors mean for business inventory planning.
5. Interactive UI & Visualizations (Streamlit)
Build an intuitive dashboard sidebar allowing the user to select the forecast horizon (30, 60, or 90 days) and filter by Product_Category.
Display high-level KPI cards at the top: Total Historical Sales, Predicted Sales for the Horizon, and Model Accuracy (100 - MAPE).
Use Matplotlib/Seaborn or Plotly to render clean, professional charts:
Historical sales vs. Model Fit vs. Future Forecasted Sales.
A breakdown of seasonal trends (e.g., average sales by month or day of the week).
Include a section that extracts "Business Insights" (e.g., "Expected demand spike detected in the next 3 weeks; recommend increasing stock levels by X%").
Deliver clean, well-commented, and robust code that I can run locally right away. Include a brief explanation of how to install dependencies and run the app.
