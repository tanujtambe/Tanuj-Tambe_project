Dataset Information
1. Fear & Greed Index Dataset
   File: fear_greed_index.csv
Records: 2,644 days
Date Range: Feb 2018 - May 2025
Columns:
timestamp: Unix timestamp
value: Index value (0-100)
classification: Fear/Greed category
date: Date in YYYY-MM-DD format

2. Historical Trading Data (Hyperliquid)
File: historical_data.csv
Records: 211,224 trades
Date Range: May 2023 - May 2025
Traders: 32 unique accounts
Assets: 246 unique coins/tokens
Key Columns:
Account, Coin, Execution Price, Size (Tokens & USD)
Side (BUY/SELL), Timestamp, Closed PnL
Fee, Leverage, Transaction details


Analysis Objectives
This project analyzes the relationship between:

Market Sentiment (Fear & Greed Index)
Trader Behavior (volume, profitability, risk)
Key Research Questions
How does market sentiment affect trading volume?
Do traders behave differently during Fear vs Greed periods?
Which sentiment conditions lead to higher profitability?
What are buy/sell patterns across different sentiments?
How do risk-taking behaviors vary with market conditions?
Which assets perform best in different market conditions?

Setup Instructions

Option 1: Google Colab (Recommended)
Open Google Colab

Upload the two CSV files:
fear_greed_index.csv
historical_data.csv
Copy the code from notebook1-analysis.md
Run all cells
Download the generated csvfiles/ and outputs/ folders

Option 2: Local Python Environment
bash
# Install required packages
pip install pandas numpy matplotlib seaborn

# Run the notebook
jupyter notebook notebook1.ipynb
Dependencies
python
pandas >= 1.3.0
numpy >= 1.21.0
matplotlib >= 3.4.0
seaborn >= 0.11.0
Analysis Workflow
Step 1: Data Loading & Preprocessing
Load both datasets

Convert timestamps to datetime

Extract time features (hour, day, month)

Create date columns for merging

Step 2: Exploratory Data Analysis (EDA)
Analyze sentiment distribution

Examine trading activity patterns

Identify unique traders and assets

Calculate basic statistics

Step 3: Data Merging
Merge trading data with sentiment data on date

Create unified analysis dataset

Date range: May 2023 - May 2025 (overlapping period)

Step 4: Trader Performance Analysis
Calculate trader-level metrics (PnL, volume, fees)

Classify traders as Profitable/Break-even/Losing

Identify top performers

Step 5: Sentiment-Based Analysis
Analyze trading volume by sentiment

Examine buy/sell ratios across sentiments

Calculate profitability by sentiment category

Identify optimal trading conditions

Step 6: Asset-Level Analysis
Identify top traded coins

Analyze coin performance by sentiment

Examine asset-specific patterns

Step 7: Advanced Insights
Time-based trading patterns (hourly)

Risk analysis (trade size categories)

Win/loss rates by sentiment

Correlation analysis

Step 8: Visualization
8 comprehensive charts covering all key findings

High-resolution PNG outputs (300 DPI)

Professional styling with clear labels

Key Findings (Sample)
Trading Volume
Highest volume sentiment: [To be determined from analysis]

Total trading volume: $XXX million

