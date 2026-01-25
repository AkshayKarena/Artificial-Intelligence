# Sales Forecasting System using XGBoost
# Project Overview
This project focuses on building a Sales Forecasting System using Machine Learning techniques.
The goal is to analyze historical sales data and predict future sales to help businesses in decision-making, inventory planning, and revenue estimation.

The model used in this project is XGBoost (Extreme Gradient Boosting) due to its high accuracy and efficiency on structured data.
# Objectives
- Analyze historical sales data
- Perform data preprocessing
- Visualize sales trends and patterns
- Train an accurate forecasting model
- Predict future sales values
# Technologies Used
# Programming Language: Python
# Libraries:
- Numpy
- Pandas
- Matplotlib/ Seaborn
- Scikit-learn
- XGBoost

# 1. Data Collection
  - Collected historical sales dataset from CSV files
# 2. Data Preprocessing
  - Handled missing values
  - Converted date columns
  - Feature scaling and encoding
# 3. Exploratory Data Analysis (EDA)
  - Sales trends visualization
  - Monthly and yearly sales analysis
  - Correlation analysis
# 4. Model Building
  - Split data into training and testing sets
  - Applied XGBoost Regression model
# 5. Model Evaluation
  - MSE
  - RAE
  - R2Score
# 6. Sales Prediction
  - Forecasted future sales based on trained model

# How XGBoost Works
  # Working Principle:
    - XGBoost builds multiple decision trees sequentially
    - Each new tree tries to correct the errors made by the previous trees
    - Instead of training all trees independently, it focuses more on wrong predictions
    - Final prediction is the sum of predictions from all trees
  # Why XGBoost?
    - High accuracy
    - Handles missing values automatically
    - Fast training using parallel processing
    - Regularization reduces overfitting

# Model Performance
  - MSE:- 963010.4375
  - MAE:- 672.5170288085938
  - R2Score:- 0.9348816871643066
