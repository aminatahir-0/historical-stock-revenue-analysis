# Historical Stock Revenue Analysis: Tesla and GameStop

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aminatahir-0/historical-stock-revenue-analysis/blob/main/historical_stock_revenue_analysis.ipynb)

---

## 📋 Abstract
This project analyzes the financial history of Tesla (TSLA) and GameStop (GME) by retrieving historical stock market data and scraping quarterly revenue records from web pages. After cleaning and organizing the datasets, the project generates clear visual comparison charts to evaluate long-term growth trends, seasonal patterns, and the correlation between business revenue and market valuation.

---

## 🛠️ Tools & Technologies Used
* **Python**: Core programming language used for data processing and script execution.
* **Pandas**: Used for data manipulation, cleaning, and DataFrame structuring.
* **BeautifulSoup (`bs4`) & Requests**: Used for fetching and parsing HTML web pages to extract financial tables.
* **yfinance**: Used for downloading historical stock market price history.
* **Matplotlib**: Used for rendering static, multi-panel comparison graphs.
* **Google Colab**: Cloud-based notebook environment used for writing and executing the code.

---

## 📐 Methodology
1. **Stock Data Extraction:** Utilized the `yfinance` library to download maximum-history share price and trading data for both companies.
2. **Revenue Data Web Scraping:** Fetched raw HTML financial pages using `requests`, parsed the document structure, and isolated quarterly revenue tables using Pandas and BeautifulSoup.
3. **Data Cleaning & Preprocessing:** 
   * Standardized table column names to `"Date"` and `"Revenue"`.
   * Stripped out unnecessary currency symbols ($) and commas from financial strings.
   * Dropped null or empty rows to ensure data integrity.
4. **Data Visualization:** Developed a custom multi-panel plotting layout using `matplotlib` to display historical share prices alongside quarterly revenue trends side-by-side.

---

## 📊 Key Observations
* **Tesla:** Demonstrated a steady, long-term upward trajectory in both revenue and stock price, with rapid acceleration and exponential growth peaking between 2019 and 2021.
* **GameStop:** Exhibited strong seasonal cyclicality in quarterly revenue (regular holiday spikes) alongside a prolonged flat stock trend followed by an unprecedented retail trading surge in late 2020 and 2021.
* **Comparison:** While Tesla's stock price closely mirrored its expanding revenue scale, GameStop experienced dramatic valuation spikes that occasionally decoupled from traditional quarterly revenue metrics.

---

## 🏁 Conclusion
By combining direct stock data extraction with web scraping techniques, this project successfully constructs clean, reliable financial datasets. The resulting visualizations provide clear insights into the contrasting growth narratives and market dynamics of Tesla and GameStop over the analyzed timeframe.
