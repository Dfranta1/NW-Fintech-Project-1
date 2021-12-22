# NW-Fintech-Project-1

## Project Background

Google Trends allows users to track the search volume of various keywords. The search volume can be subdivided into geographic zones. It is hypothesized that by tracking search volume of keywords, one could develop a market sentiment indicator that would enable above market returns, alpha. A first round of analysis would involve a visual inspection of the data, to be followed by a more rigorous statistical analysis. This project is limited to the first round of analysis, where stock price movement is plotted against keyword search volume. But wait, there is more! We enhanced the project by adding Bollinger Band analysis.

Bollinger Band analysis is a technical model that plots a simple moving average of security prices within two volatility defined bands. The upper band is set by adding two standard deviations to the moving average and the lower band is set by subtracting 2 standard deviations from the simple moving average. 
The use of Bollinger Bands in this analysis is to see if the volatility of a stock’s price matched the same period of positive or negative sentiment trends, thereby evaluating google trends as a sentiment analysis as an effective trading strategy.

Google Trends  does not provide the whole universe of google searches, but rather a sampling of all searches. Google maintains that this sample is representative of the whole search universe. There is no material loss of information by doing such. Google Trends normalizes search data. Google describes the normalization process as follows:
Each data point is divided by the total searches of the geography and time range it represents to compare relative popularity. Otherwise, places with the most search volume would always be ranked highest. The resulting numbers are then scaled on a range of 0 to 100 based on a topic’s proportion to all searches on all topics.
Different regions that show the same search interest for a term don’t always have the same total search volume.

Google Trends monitors search for automated search activity in the attempt to spam search results. “While we have mechanisms in place to detect and filter irregular activity, these searches may be retained in Google Trends as a security measure, filtering them from Google Trends would help those issuing such queries to understand we’ve identified them.” Note, Google does remove suspicious searches in their autocomplete function.

Google Trends should not be considered Polling Data, it is not a scientifically designed sample.

### Keywords used
*Note: Any sample of key words can be used*


- Unemployment

- Recession

- Bear Market

- Downturn

- Economic Downturn

- Covid

- Buy Stocks

- Sell Stocks

- Mortgage Rates

- Cruise

- Remodeling

- Jewelry


### Stocks used 
*Note: Any sample of stocks can be used*

- Apple

- Microsoft

- JP Morgan

- Bank of America

- Pfizer

- Johnson & Johnson

- Coke

- Campbells Soup

- Caterpillar

- Honeywell

### Built with

PyViz

Panel

Plotly

Pandas

Hvplot

Matplotlib

Numpy

Dotenv

Sklearn

MinMaxScaler

Alpaca trade api

Yfinance

Pytrends

Scipy

Holoviews

## Getting Started

### Installations

**Scipy**
>python -m pip install --user numpy scipy matplotlib ipython jupyter pandas sympy nose


**Scikit Learn**
>conda create -n sklearn-env -c conda-forge scikit-learn
>conda activate sklearn-env


**Pytrends**
>pip install pytrends


**YFinance**
>pip install yfinance


**Alpacas**

All packages should be installed into the alpacaenv virtual environment. To create the alpacaenv virtual environment, run the following command in your terminal, answering y when prompted:

 >conda create -n alpacaenv python=3.7 anaconda


After the alpacaenv environment installation is complete, activate it by typing the following command:

 >conda activate alpacaenv


Next, install the python-dotenv package by running the following command in your terminal:

>pip install python-dotenv


Now, initiate the alpaca-trade-api install by running the following command:

>pip install alpaca-trade-api


Go to Alpaca Markets and log into your account. After logging in you may be taken to a form asking you for personal information - **YOU DO NOT NEED TO ENTER THIS INFORMATION.**

Now, click the Go to Paper Account link in the navigation sidebar.
Now click on the Your API Keys section and grab your ALPACA_API_KEY and ALPACA_SECRET_KEY.
Next, create a new file named .env. This is where you will store your keys.


Using the syntax in the image below, create your environment variables inside the .env file. NOTE: Make sure your environment variables are specifically named ALPACA_API_KEY and ALPACA_SECRET_KEY.



