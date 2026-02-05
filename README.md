# Phase One: Data Collection and Preparation

## Project Overview
This repository contains Phase One of a Stock Market Portfolio Optimization and Forecasting System.
Phase One focuses on collecting, cleaning, and preparing stock market data so it can be used reliably in later phases for portfolio construction, risk analysis, and forecasting.

## Objectives of Phase One
The key objectives of this phase are:
- To collect historical stock price data from public data sources
- To clean and align the data into a consistent format
- To calculate daily returns for each asset
- To prepare a structured dataset suitable for analysis and modeling.

## Data Time Period
The historical price data used in this phase covers approximately daily trading for each asset.
For the datasets generated so far, the time period shown in the visualizations is roughly 04-Nov-2025 to 07-Feb-2026.  
Data is downloaded dynamically from YFinance at the time the scripts are executed, so future runs may have slightly different date ranges.
This ensures that the dataset is up to date, reproducible, and suitable for analysis, while keeping the visualizations neat and readable.

## Asset Universe Used. 
- Apple Inc. (AAPL)
- Microsoft Corporation (MSFT)
- NVIDIA Corporation (NVDA)
- JPMorgan Chase & Co. (JPM)
- S&P 500 Index (^GSPC) – Global market benchmark
### Local Market Context (Kenya)
- Safaricom PLC
- Equity Bank Group
- Nairobi Securities Exchange 20 Index (NSE 20)
Due to data availability limitations on YFinance, Kenyan equities are not directly included in the downloaded datasets for this phase. Placeholders are maintained to preserve a global–local portfolio structure and allow seamless inclusion of official NSE data in later phases.

## Folder Structure Explanation
Phase-One/

│
├── Data/
│ ├── Raw/ → Raw stock price data downloaded from YFinance
│ └── Processed/ → Cleaned datasets and calculated daily returns
│
├── Scripts/
│ ├── download_data.py → Downloads historical stock price data
│ ├── process_data.py → Cleans data and computes daily returns
│ └── plot_charts.py → Generates visualizations
│
├── Output/
│ └── Charts and visual outputs.

### Daily Closing Prices (Nov 2025 – Feb 2026)
Below is the line chart showing the daily closing prices of selected global assets.  
It shows the trend of each asset over the 3-month period for easier comparison.
![Daily Closing Prices](Output/closing_prices_line.png)

Future phases will include:
- Integration of official Kenyan market data
- Portfolio allocation and optimization models
- Risk analysis and forecasting techniques

Results and visualizations may change when the data is refreshed due to differences in market conditions and time periods.

## Disclaimer
The data used in this project is sourced from publicly available financial data providers and is used strictly for educational and learning purposes.
This project does not constitute financial advice. Any analysis or results are intended solely to demonstrate data analysis techniques and should not be used for investment decision-making.


