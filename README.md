# Finance Projects Overview
* ## Stock price prediction Project (Regression)
* ## Stock prediction Project (Classifier)

* Created a tool that estimates stock prices.
* Scraped the most active stocks' 5 year history data from yahoo finance using python.
* Tried
* Used Prophet, Random Forest and Gradient Boosting model.

## Code
* Python 3 (ipykernel)
* Packages: pandas, numpy, sklearn, matplotlib, seaborn, plotly, json, bs4, requests, csv, re, io, yfinance, prophet

## Web Scraping
Write a web scraper to scrape the most active stocks' symbol and history data. I got the following data:
* Date
* Open
* High
* Low
* Close
* Voolume
* Price
* Dividens
* Stock splits

## Stock price prediction Project (Regression)
## Model Building
First, I droped the Volume and Stock Splits columns. Date column is the index.

After that I split the dataset into a train (first x-100 data) and test (last 100 data) datasets.


I tried three different models:
* Linear Regression - Baseline for the model
* Random Forest Regressor
* Gradient Boosting Regressor

## Model performance
The random Forest and Gradient Boosting Regressor model got a 0.96 score, probably overfitting occured.
![Performance](https://github.com/trauerj/Finance_Project/blob/main/image.png)
## Conclusion
This type of project is good for practice plots and models writing, but not have a real life use.

## Stock prediction Project (Classifier)
In this project I want to predict if the stock price will rise  or fall using Random Forest Classifiermodel, and backtesting.
## Model Building
First, I droped the Volume and Stock Splits columns. Date column is the index.

After that, I made new column "Tommorrow" which is shifted Close column and new column "Target" as int wich value depends on Tommorrow greater or not than Close.

Predictors are the remaining columns excluding "Tommorrow". (Naturally)

The split method is the same as in the other project. (train first x-100 row; test  last 100 row)
.
.
.
