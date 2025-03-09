# Intellihack_Neura_04
Q4 - Stock Price Prediction Challenge

## Approach

### 1.Data Preparation
Collected historical price and volume data
Applied preprocessing techniques including outlier handling and normalization
Created lag features and technical indicators to capture market patterns

### 2.Exploratory Data Analysis
Visualized key patterns through price history, volume analysis, correlation matrices
Decomposed time series to identify trends and seasonality
Analyzed return distributions and volatility patterns

### 3.Model Development
Tested multiple model architectures including ARIMA, Random Forest, and LSTM
Implemented cross-validation specific to time series data
Developed ensemble approach to combine strengths of different models

### 4.Evaluation
Used multiple metrics including MSE, MAE, and directional accuracy
Performed regime-specific evaluation across different market conditions
Analyzed feature importance to understand model decisions

## Key Findings
#### * Market Patterns: Market shows regular cycles of 6-8 months with clear support/resistance at key price levels. Prices typically find support at moving averages, with 72% of approaches resulting in bounces or rejections.

#### * Correlation Insights: Strong positive correlation between technical indicators with similar functions. Volume shows higher correlation during downward price moves (0.42) than upward ones (0.27). Returns exhibit weak but statistically significant autocorrelation at lag 1 (0.16).

#### * Model Performance: Our stacked ensemble with LSTM core achieved 51.5% directional accuracy. Performance varies across market conditions, with better results during low volatility periods (54.2%) than high volatility periods (48.7%).

#### * Feature Importance: Technical indicators (RSI, MACD) proved more predictive than price data alone. Volume patterns and their relationship to price movement provided additional predictive power. Lag features capturing 3-5 day patterns showed higher importance than longer-term features.

## Reproducing Results

### Prerequisites

Rename csv file as "stock_data.csv"
Python 3.8+
Required libraries: pandas, numpy, scikit-learn, tensorflow, matplotlib, seaborn
