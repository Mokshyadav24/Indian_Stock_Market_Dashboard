# Stock Trading Report

This repository contains a **Stock Trading Report** created using Power BI. The report provides a detailed analysis of stock performance over time, covering various key metrics such as open, close, high, and low prices. It is designed to help traders and analysts gain insights into stock market trends and make informed decisions.


## Overview

The report includes the following features:

- **Stock Performance Dashboard**: Visualizes the performance of multiple stocks such as AXISBANK, HDFCBANK, ICICIBANK, and more.
- **Historical Data Analysis**: Tracks the open, close, high, and low prices for each stock over a specific period.
- **Interactive Visuals**: Provides interactive charts and graphs that allow users to explore data by different time frames (e.g., 1Y, 3M, 5D, etc.).
- **Comparative Analysis**: Enables comparison of stock performance across different time periods and between different stocks.

![Stock Trading Report Dashboard](https://i.postimg.cc/Jh0vVqcG/Stock-Treding-Report-black-page-0001.jpg)
![Stock Trading Report Dashboard](https://i.postimg.cc/cCyb3Nqn/Stock-Treding-Report-black-page-0002.jpg)
![Stock Trading Report Dashboard](https://i.postimg.cc/L4L7phfB/Stock-Treding-Report-White-page-0001.jpg)

## Technology Used

- **Power BI Desktop**: The report was created using Power BI Desktop, a business analytics service by Microsoft. Power BI allows for data preparation, data discovery, and interactive reporting.
- **API Integration**: Data was fetched using an external API to ensure the most up-to-date stock information is used in the report.

## Setting Up the API Key

To fetch the stock data, you need to have an API key from the data provider. Follow these steps to set it up:

1. **Obtain an API Key**: 
   - Sign up at the API provider's website use Yahoo Finance
   - Obtain your API key from your account dashboard.

2. **Insert API Key in Power BI**:
   - Open the Power BI report file (`.pbix`).
   - Go to **Transform Data** -> **Advanced Editor** in Power BI Desktop.
   - Locate the line where the API URL is defined and insert your API key. It might look like this:
     ```m
     let
         Source = Json.Document(Web.Contents("https://api.example.com/data?symbol=AAPL&apikey=YOUR_API_KEY"))
     in
         Source
     ```
   - Replace `YOUR_API_KEY` with the actual API key you obtained.

3. **Refresh the Data**:
   - Once the API key is set, refresh the dataset to pull in the latest stock data.




## Contact

For any questions or feedback, feel free to reach out at mokshyadav.024@gmail.com.
