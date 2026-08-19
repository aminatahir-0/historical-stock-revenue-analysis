# 📈 Financial Data Analysis & Web Scraping: Tesla and GameStop

[![Open In Colab](https://colab.research.google.com/github/aminatahir-0/historical-stock-revenue-analysis/blob/main/historical_stock_revenue_analysis.ipynb)

---

## 📋 Abstract
This project analyzes the financial history of Tesla and GameStop by gathering stock market data through APIs and scraping quarterly revenue details from web pages. After cleaning and organizing the data, it generates clear comparison charts to help examine long-term growth trends, seasonal patterns, and the relationship between business revenue and stock value.

---

## 🛠️ Tools & Technologies Used
* **Python**: Core programming language used for data processing and automation.
* **Pandas**: Used for data manipulation, cleaning, and DataFrame structuring.
* **BeautifulSoup (`bs4`) & Requests**: Used for fetching and parsing HTML web pages to extract financial tables.
* **yfinance**: Used for downloading historical stock market data.
* **Matplotlib**: Used for rendering static, multi-panel comparison graphs.
* **Google Colab**: Cloud-based notebook environment used for writing and executing code.

---

## 📐 Methodology
1. **Data Extraction (Stock Market):** Utilized the `yfinance` library to pull maximum available historical stock price and trading data for both Tesla and GameStop.
2. **Data Extraction (Revenue Web Scraping):** Downloaded raw HTML pages containing financial data using `requests`, inspected the page structures, and isolated the relevant quarterly tables using Pandas and BeautifulSoup.
3. **Data Cleaning & Preprocessing:** 
   * Standardized column names to `"Date"` and `"Revenue"`.
   * Used regular expressions (`regex`) to strip out currency symbols ($) and commas from financial strings.
   * Dropped null/empty rows to maintain data integrity.
4. **Data Visualization:** Developed a custom multi-panel plotting workflow using `matplotlib` to display historical share prices alongside quarterly revenue trends for comparative analysis.

---

## 📊 Key Observations
* **Tesla:** Demonstrated a steady, long-term upward trajectory in both revenue and stock price, with rapid acceleration and exponential growth peaking between 2019 and 2021.
* **GameStop:** Exhibited strong seasonal cyclicality in quarterly revenue (regular holiday spikes) alongside a prolonged flat stock trend followed by an unprecedented retail trading surge in late 2020/2021.
* **Comparison:** While Tesla's stock price closely mirrored its expanding revenue scale, GameStop experienced dramatic valuation spikes that occasionally decoupled from traditional quarterly revenue metrics.

---

## 🏁 Conclusion
By combining stock APIs and web scraping, this project successfully builds clean datasets to compare and visualize real-world financial trends for both companies.
