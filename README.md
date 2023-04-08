# mit-ids-stock-news-significance
IDS.012 is a hands-on data analysis course at MIT that introduces the interplay
between statistics and computation for the analysis of real data. The class includes a final project that is done in small groups. Our group has chosen a project that aims to quantify the impact of breaking news articles on stock performance. By analyzing news sentiment, we can better understand the market's reaction to news and make informed trading decisions.

## Idea and Motivation
It is well-established that breaking news articles/headlines can directly impact a company's stock performance. However, more work is needed to quantify this effect. A better understanding of the market's reaction to news sentiment is instrumental in informing trading decisions. We seek to tackle this problem in 4 parts:

1. Cluster equities (we will likely focus on companies in the S&P 500) based on how they trade (volatility, 52-week high and low, market cap, etc.), company financials (revenue, operating income, cash flows, etc.), as well as sector (technology, industrial, consumer discretionary, etc.).
2. Perform hypothesis testing to identify which moves in a stock's prices are deemed significant.
3. Use [Newscatcher News API](https://newscatcherapi.com/) to pull news articles and quantify their sentiment (using a python natural language processing package such as NLTK).
4. Combine the work from the first three parts to quantify the impact of news sentiment on stock performance.

## Data
For this project, we need news articles sorted by the company as well as company trading data and financials. We will use [Newscatcher News API](https://newscatcherapi.com/) to acquire the news articles. Company trading data and financials will be obtained using Yahoo Finance.

## Analysis Methods
We will be exploring the data using various analysis methods we learned in class. To cluster equities based on different variables, we will be using methods such as the k-means algorithm as well as t-SNE. For the hypothesis testing we will be using libraries in python to model the normal distribution and the  various correction methods to account for multiple hypotheses. We will also explore the data using feature selection methods such as the backward selection model and L1 regularization to evaluate which features we are using to cluster the equities. This is where much of the preprocessing of our data will happen. 
We will be using natural language processing libraries in python (i.e., NLTK) to qualify the sentiment of articles surrounding a company to see how that impacts the performance of the equity. 
