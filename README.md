# Apple Stock Performance During COVID-19

## 1. Problem & User
**Problem**: How did Apple's stock price react to the COVID-19 crash and how quickly did it recover?  
**Target user**: Beginner investors who want to understand market behavior during crises.

## 2. Data
- **Source**: WRDS CRSP Daily Stock File (`crsp.dsf`)
- **Access date**: April 12, 2026
- **Company**: Apple Inc. (PERMNO 14593)
- **Time period**: 2018-01-01 to 2023-12-31
- **Key variables**: `date`, `ret` (daily return), `prc` (price)

## 3. Methods
- SQL query to retrieve data from WRDS
- Data cleaning with pandas (date conversion, missing values)
- Calculate cumulative return (indexed to 100) and 30-day rolling volatility
- Identify maximum drawdown and recovery date
- Visualizations: cumulative return line chart, volatility line chart

## 4. Key Findings
- Apple stock dropped **38%** from pre-COVID peak to March 23, 2020 bottom.
- Fully recovered to pre-crisis level by **August 2020** (only 5 months).
- Volatility spiked from <2% to >8% during the crash, then normalized.
- By end of 2023, cumulative return more than doubled.

## 5. How to Run
1. Clone this repository or download the notebook.
2. Install dependencies: `pip install -r requirements.txt`
3. Open `apple_analysis.ipynb` in Jupyter Notebook.
4. Run all cells (requires WRDS credentials).

## 6. Demo Video
[Click here for demo video](https://your-video-link.com)

## 7. Limitations & Next Steps
- Only stock returns, no fundamental data (revenue, profit).
- No benchmark comparison (e.g., S&P 500).
- Future work: add market index, include Compustat fundamentals.
