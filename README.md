# bitcoin-sentiment-trader-analysis
Market sentiment analysis using the Bitcoin Fear &amp; Greed Index and Hyperliquid trading data to study the relationship between trader performance, trading activity, and market psychology.
# Bitcoin Sentiment Trader Analysis

## Overview

This project analyzes the relationship between **Bitcoin market sentiment** and **trader performance**.
By combining the **Fear & Greed Index dataset** with **Hyperliquid historical trading data**, the project explores how market psychology influences trading outcomes such as profitability, activity, and volatility.

The goal is to identify patterns that could help traders and analysts understand how **market sentiment impacts trading behavior**.

---

## Objective

The main objectives of this project are:

* Study the relationship between **market sentiment (Fear vs Greed)** and trader profitability
* Analyze how **trading activity changes under different sentiment conditions**
* Measure **profit volatility during fear and greed markets**
* Evaluate **win rate patterns across sentiment states**
* Generate insights that may support **better trading strategies**

---

## Datasets Used

### Bitcoin Fear & Greed Index

This dataset represents the overall sentiment of the Bitcoin market.

**Columns include**

* timestamp
* value
* classification (Fear / Greed)
* date

Dataset source
https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view

---

### Hyperliquid Historical Trader Data

This dataset contains detailed records of trading activity on the Hyperliquid platform.

**Columns include**

* Account
* Coin
* Execution Price
* Size Tokens
* Size USD
* Side
* Timestamp IST
* Start Position
* Direction
* Closed PnL
* Fee
* Trade ID
* Timestamp

Dataset source
https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view

---

## Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* gdown

---

## Project Workflow

### Data Import

Datasets are downloaded directly from Google Drive using **gdown**.

### Data Cleaning

* Standardizing column names
* Converting timestamps to datetime format
* Handling missing values

### Feature Engineering

* Creating win/loss indicators
* Extracting trading dates
* Generating daily trading statistics

### Data Aggregation

Trade-level data is aggregated into **daily trading metrics**.

### Dataset Merging

Trading statistics are merged with the **Fear & Greed sentiment dataset** using the date column.

### Exploratory Data Analysis

The project analyzes:

* Profit vs Market Sentiment
* Trading Activity vs Sentiment
* Trading Volume vs Sentiment
* Win Rate vs Sentiment
* Profit Volatility

---

## Key Metrics Analyzed

* Daily Profit / Loss (PnL)
* Trade Count
* Trading Volume
* Win Rate
* Profit Volatility
* Market Sentiment

---

## Key Insights

* Traders tend to generate **higher profits during Greed periods**.
* **Trading activity increases** when the market sentiment is positive.
* **Fear markets show higher volatility**, indicating unstable price movements.
* **Win rates tend to decrease during Fear conditions**, suggesting greater uncertainty.

These observations indicate that **market sentiment significantly influences trading behavior and outcomes**.

---

## How to Run the Project

1. Open the notebook in **Google Colab**
2. Install required libraries

pip install gdown pandas numpy matplotlib seaborn

3. Run all notebook cells sequentially
4. The datasets will automatically download from Google Drive

---

## Project Structure

bitcoin-sentiment-trader-analysis
│
├── bitcoin_market_sentiment_trader_performance_analysis.ipynb
└── README.md

---

## Future Improvements

Possible extensions of this project include:

* Building a **machine learning model** to predict profitability using sentiment
* Performing **individual trader performance analysis**
* Studying **risk behavior and leverage usage**
* Integrating additional market indicators

---

## Author

Anshu Dagur

---

## Conclusion

This project demonstrates how **market sentiment can influence trader behavior and profitability**. By combining sentiment indicators with trading data, analysts can gain deeper insights into **market psychology and decision-making patterns**.
