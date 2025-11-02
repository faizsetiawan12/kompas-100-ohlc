# Indonesia Stock OHLC Data Repository

This repository contains historical Open, High, Low, Close (OHLC) and Volume data for Indonesian stocks.

## Data Structure

Each stock has its own CSV file located in the `data/historical/` directory. The file naming convention is `\{TICKER\}.csv` (e.g., `BBCA.csv`, `TLKM.csv`).

### Format

The CSV files follow this specific format:
- First row: `Price,Close,High,Low,Open,Volume`
- Second row: `Ticker,\{TICKER\}.JK,\{TICKER\}.JK,\{TICKER\}.JK,\{TICKER\}.JK,\{TICKER\}.JK`
- Third row: `Date,,,,,`
- From fourth row onwards: Date, Close, High, Low, Open, Volume

### Columns
- Date: In YYYY-MM-DD format
- Open: Opening price
- High: Highest price during the day
- Low: Lowest price during the day
- Close: Closing price
- Volume: Trading volume

## Data Sources

Data is collected from various sources including Yahoo Finance and Indonesian broker data.

## License

This data is made available under the MIT License.

## Last Updated

Data is current through October 31, 2025.

## Usage

These CSV files can be directly loaded into pandas DataFrames or other data analysis tools for financial analysis, backtesting, and research.
