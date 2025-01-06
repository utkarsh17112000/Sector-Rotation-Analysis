# Sector Movement Analysis

This project aims to analyze and predict sector rotation patterns in the Indian stock market by leveraging NIFTY indices data. The analysis incorporates data visualization, statistical insights, and machine learning models to provide actionable insights into market trends. The project also includes interactive Tableau dashboards to present the data intuitively for stakeholders.

# Key Features

## Data Collection:

-Downloaded historical data for various NIFTY indices (e.g., NIFTY50, Bank NIFTY, FMCG NIFTY, etc.) using the yfinance library.

-Indicators included: Adj Close, Close, High, Low, Open, Volume, Daily Returns, Weekly Returns, Monthly Returns, 10-Day MA, 50-Day MA, Volatility.

## Data Preprocessing:

-Filled missing values using forward fill to ensure consistency in the time series data.

-Standardized all datasets to ensure uniformity for machine learning models.

## Feature Engineering:

-Calculated key indicators: Moving Averages (10-day and 50-day), Daily, Weekly, and Monthly Returns.

-Derived volatility measures for risk assessment.

## Data Visualization:

-Visualized key indicators (Close prices, Moving Averages, and Returns) using Python libraries like matplotlib and seaborn.

-Created sector-wise correlation heatmaps.

-Interactive Tableau dashboard for presenting insights, such as:

1. Sector-wise performance trends.
   
2. Key Moving Averages and Volatility.
   
3. Comparisons across indices.

## Machine Learning Models:
-Implemented predictive models to forecast sector indices.

-Models used: Bayesian Ridge Regression, Linear Regression, Random Forest, and XGBoost.

-Evaluation metrics: Mean Squared Error (MSE) and R-squared.

## Integration:
-Combined all processed datasets into a single CSV for Tableau visualization.

-Incorporated separate CSVs for individual sectors while ensuring compatibility with Python and Tableau.


# Steps in the Project

## 1. Data Collection

-Libraries used: yfinance, pandas.

-Historical data for indices downloaded using yfinance.download().


## 2. Data Preprocessing

-Removed missing values using data.fillna(method='ffill').

-Standardized columns across datasets.


## 3. Feature Engineering

-Added calculated fields like:

-Moving Averages: rolling(window=10).mean().

-Returns: pct_change().

-Volatility: Standard deviation over a rolling window.


## 4. Data Visualization

### Python Visualizations:

-Line charts for Close prices and Moving Averages.

-Area charts for trend comparisons.

-Bar charts for Weekly Returns.

-Correlation heatmap for sector-wise analysis.


### Tableau Dashboard:

-Interactive visualizations for stakeholders.

-Filters for sector-specific insights.


## 5. Machine Learning

-Prepared training and test datasets for individual indices.

-Implemented machine learning models for predictions.

-Used Bayesian Ridge Regression for predictive modeling alongside other algorithms.

-Evaluated results and compared metrics.


## 6. Integration

-Saved processed data into CSV files.

-Imported combined datasets into Tableau for dashboard creation.


# Tools and Technologies

-Data Collection: Python (yfinance, pandas)

-Data Preprocessing & Feature Engineering: Python (numpy, pandas)

-Data Visualization: Python (matplotlib, seaborn), Tableau

-Machine Learning: Python (scikit-learn, xgboost)

-Dashboard: Tableau

