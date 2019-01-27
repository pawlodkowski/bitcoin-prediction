# Overview
---

### This repository contains 2 iPython (Jupyter) notebook files:
1. The primary file, `BitcoinPricePrediction.ipynb`, which serves as a tutorial for predicting the price of Bitcoin (2 days in the future) based on data pulled from the [CoinGecko API](https://www.coingecko.com/api/docs/v3).
2. A secondary file, `MakingPredictionsWithModel-Demo.ipynb`, which further breaks down Step 5 of the primary file (i.e. the code that is used to generate the DataFrame used as the "test data set" for making the actual prediction).

# Task:
---

The task is to train a linear regression model to predict what the price of Bitcoin will in 1-2 days. The features used in the model are mostly historical prices of Bitcoin and other cryptocurrencies (e.g. BTC price from 2 days ago, ETH price from 2 days ago) as well as "community data" (e.g. social media-related statistics) that can be extracted from the CoinGecko API.  

This notebook includes examples of various data analysis, modeling, and visualization techniques that can be used to solve the problem using Python. The purpose of this file is not to predict the most accurate price of Bitcoin in the future (cryptocurrency prices are inherently volatile / wildly unpredictable) nor to thoroughly teach financial time series analysis and statistics, but rather to be used as a guide for teaching students introductory data analysis and web-scraping tools in Python. These tools and strategies include:
- "Wrangling" data in *pandas* and applying features engineering to a data set.
- Visualzing data in *matplotlib* and *seaborn* to inform optimal feature selection.
- Training 3 types of classification models (*Linear Regression*, *Ridge Regression*, *Lasso Regression*) on the data set and using them to make predictions.
    - In the preceding lectures, the students will get a more in-depth, theoretical understanding of how regularization works, why it is used, and how it affects the resulting model's coefficients.
- Using *requests* in Python to learn how to extract your own data from the internet; in this case, a relatively simple API that outputs clean data in JSON format and does not require any authentication.
---

## TO-DO:

A more rigorous analysis of the financial time series data can be explored with the *statsmodels* library in Python. Models to be added in a future notebook:
- Exponential Smoothing
- Autoregressive-moving-average (ARMA).
