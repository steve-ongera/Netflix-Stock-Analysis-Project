# Netflix Stock Analysis Project

## Overview
This project performs comprehensive analysis of Netflix (NFLX) stock data from 2015 to 2024 using Python in a Jupyter Notebook environment. The analysis includes price trends, moving averages, daily returns, volatility, and correlation analysis.

## Prerequisites
- Python 3.x
- Jupyter Notebook
- Required libraries:
  - yfinance
  - pandas
  - matplotlib
  - seaborn

## Installation
```bash
# Install Jupyter Notebook if you haven't already
pip install notebook

# Install required libraries
pip install yfinance pandas matplotlib seaborn
```

## Running the Notebook
1. Open terminal/command prompt
2. Navigate to the project directory
3. Run:
```bash
jupyter notebook
```
4. Open `netflixstockanalysis.ipynb` in the Jupyter interface

## Project Structure
The analysis is contained in a single Jupyter Notebook (`netflixstockanalysis.ipynb`) with the following major components:

1. Data Collection
   - Fetches historical stock data using yfinance
   - Time period: 2015-01-01 to 2024-01-01
   - Downloads OHLCV (Open, High, Low, Close, Volume) data

2. Data Analysis
   - Basic data exploration
   - Statistical analysis
   - Moving averages calculation
   - Daily returns computation
   - Volatility analysis

3. Visualizations
   - Stock price trends
   - Moving averages (50-day and 200-day)
   - Daily returns
   - Volume vs Returns scatter plot
   - Correlation heatmap
   - Volatility trends

## Notebook Sections

### 1. Data Collection
- Uses `yfinance` to download Netflix stock data
- Stores data in a pandas DataFrame
- Performs initial data validation

### 2. Basic Data Exploration
- Displays basic information about the dataset
- Checks for missing values
- Generates descriptive statistics

### 3. Price Analysis
- Plots closing price over time
- Calculates and visualizes:
  - 50-day moving average
  - 200-day moving average

### 4. Returns Analysis
- Calculates daily returns
- Visualizes return distribution
- Analyzes relationship between volume and returns

### 5. Correlation Analysis
- Creates correlation matrix
- Visualizes correlations using heatmap
- Analyzes relationships between different price metrics

### 6. Volatility Analysis
- Calculates standard deviation of returns
- Plots 21-day rolling volatility
- Provides volatility insights

### 7. Data Export
- Saves processed data to 'netflix_stock_analysis.csv'
- Includes all calculated metrics and indicators

## Output Files
- `netflix_stock_analysis.csv`: Contains all processed data and calculations
- Various plots and visualizations are displayed inline in the notebook

## Data Dictionary
- **Open**: Opening price for the day
- **High**: Highest price during the day
- **Low**: Lowest price during the day
- **Close**: Closing price for the day
- **Volume**: Number of shares traded
- **50_day_ma**: 50-day moving average of closing price
- **200_day_ma**: 200-day moving average of closing price
- **Daily_Return**: Percentage change in closing price from previous day

## Jupyter Notebook Tips
- Run cells in sequential order to ensure proper execution
- Use "Restart & Run All" to reset and execute all cells
- Markdown cells provide explanations for each analysis step
- Code cells can be modified to adjust analysis parameters

## Notes
- All dates are in YYYY-MM-DD format
- Prices are in USD
- Moving averages use closing prices
- Volatility is calculated using 21-day rolling window
- Visualizations are interactive in the Jupyter environment

## Future Improvements
1. Add more technical indicators
2. Implement predictive modeling
3. Add automated reporting features
4. Include real-time data updates
5. Add risk metrics calculations
6. Export visualizations as separate image files
7. Add interactive widgets for date range selection

## Troubleshooting
- If you encounter display issues, try:
  ```python
  %matplotlib inline
  ```
- For memory issues, restart the kernel and run cells one by one
- Ensure all required libraries are installed before running

## License
+254 112284093