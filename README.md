## In a nutshell

This project takes input from user and generate's financial report. It generate links through internet search API DuckDuckGo, filters only finance.yahoo website links. Extract symbol from weblink using regex, pass it in yfinance python library as ticker and generate financial charts and reports. The final output has csv file which contains yearly and quaterly financials of the comany.

## Steps

In this project I have analysed Canoo INC. Canoo is an electric automotive company based in US. It was founded by Ulrich Kranz in 2017. Canoo's mission is to make electric
vehicles (EVs) available to everyone. Canoo's goal is to lead the automotive industry's transition to clean and sustainable energy.

Canoo offers a variety of vehicles, including
Lifestyle Delivery Vehicle (LDV)
American Bulldog Pickup.
Canoo EV fleet.
Modular electric platform. 

Canoo has Market cap of $156,933,008 and is competing with Rivian Automotive, Fisker and Lucid group.


My Approach goes by:

1.DuckDuckGo API Search:

Use the DuckDuckGo API to search for links related to Canoo.

2.Filter yfinance Web Links:

Filter the links to keep only those related to yfinance.

3.Extract Ticker using Regex:

Apply regex to extract the ticker symbol from the link.

4.Use Ticker with yfinance Library:

Provide the extracted ticker to the yfinance library.

5. Extract Financials:

Fetch financial data using yfinance.

6.Identify Keys for Extraction:

Identify specific keys or data columns to be extracted from the financial data.

7.Find Similar Companies:

Use the URL from external website to find symbols of similar companies.

8.Extract Symbols for Tickers:

Extract ticker symbols for identified similar companies.

9.Filter Available Tickers in yfinance:

Not all companies information is available in yfinance library, hence filter out tickers for which data is available in the yfinance database.

10.Extract Historical Data

Use yfinance to extract historical data for the identified tickers.

11.Plot Graphs on Financial Data:

Create plots and graphs based on the financial data.

11.Identify Competitors and Plot Data:

Identify competitors from the extracted symbols and plot their financial data.

12.Save to CSV:

Save the extracted and processed data to a CSV file.


## Summary

According to The Motley Fool, Canoo used to be a Wall Street darling during the early part of the COVID-19 pandemic, but investors have mostly given up on GOEV for their own good, as the stock is losing its value. The company's ebitda has been increasing since 2022 despite no revenue being generated. The company only turned a profit in 2020 was about $1,880,000. The company has lost everything since then. According to reports, it's because of internal disputes, departures, and financial investments in underutilised infrastructure.

To address this issue I started using the Beautifulscop Python Library with Scrapy. It didn't produce any results when I applied it on the Nasdaq website. The main reason for this was that the Nasdaq website was dynamic, meaning that data was updated every minute.

I learned about the Yfinance Library later. It is used for financial analysis using pyton. It seemed like the best source to go from there. Using this library, I examined Canoo's whole financial records, created graphs, and researched its competitors. Later, I started working on the Internet Search API and extracted finance.yahoo website's links from it. I then used regex to extract symbols that are present in the later part of the weblink. I was able to save the data in CSV format and solve every problem in the problem statement by using this method.
