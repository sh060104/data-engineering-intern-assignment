# data-engineering-intern-assignment
Monthly stock aggregation with SMA &amp; EMA using Pandas
Stock Data Monthly Processor
Overview
A Python-based data pipeline that converts daily stock price data into monthly summaries and calculates technical indicators (SMA and EMA).

How to Run
Install dependencies: pip install pandas

Place datastock_data.csv in the project folder.

Run the script: python main.py

Assumptions & Logic
OHLC Logic: "Open" is the first trading day of the month; "Close" is the last. "High" and "Low" are the absolute max/min for the month.

Indicators: SMA and EMA (periods 10 and 20) are calculated on the monthly closing prices.

EMA Seed: The first EMA value uses the first available closing price as the starting point.

Output: Generates 10 separate CSV files, each with 24 rows representing 2 years of data.
