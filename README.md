# Pairs Trading: A Statistical Arbitrage Strategy

## Basic Idea
- Select two stocks which move similarly.
- Find where the price diverges.
- Sell the high priced stock and buy the low priced stock.
- The idea is to capture absolute return regardless of market fluctuations.

### 

## Getting data


- Get daily closing prices for a universe of stocks --> Alpha Vantage


- Include other company information (sector, profitability, debt ratios, etc.) --> Yahoo! Finance & Wikipedia

### 

## Finding suitable pairs 
(January 4, 2016 - December 31, 2018)


- Use a clustering technique on the universe of stocks
    - Possibly K-means, but possibly DBSCAN or hierarchical
    - Use PCA before the clustering to reduce dimensionality
    - Dimensions will be price return each day, sector, market cap, etc.
    

- Find suitable pairs in each cluster
    - Need to determine that each pair moves similarly
        - Calculate the cointegration of each pair
        - Find out if the spread of each pair is stationary

### 

## Mock trading over a year 
(January 2, 2019 - December 31, 2019)


- Identify entry and exit points in the strategy for a pair over a year

### 
