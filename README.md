# Trading systems development Project Overview
* 
* 
* 

## Code
* Python 3 (ipykernel)
* Packages: pandas, numpy, sklearn, matplotlib, seaborn, plotly, json, bs4, requests, csv, re, io, yfinance, prophet

## Model Building
First, I droped the Volume and Stock Splits columns. Date column is the index.

After that I split the dataset into a train (first x-100 data) and a test (last 100 data) datasets.


I tried three different models:
* Linear Regression - Baseline for the model
* Random Forest Regressor
* Gradient Boosting Regressor

## Model performance
The Random Forest and Gradient Boosting Regressor model got a 0.96 score.

![Performance](https://github.com/trauerj/Finance_Project/blob/main/image.png)
_**This figure shows us the predictions compared to the real values (test set).**_

## Conclusion
This type of project is good for practicing different type of plots (libraries/packeges) and models (E.g. prophet), but not usable in real life scenarios.

# Stock prediction Project (Classifier)
In this project I want to predict if the stock price will rise  or fall using Random Forest Classifier model, and backtesting.
## Model Building
First, I droped the Volume and Stock Splits columns. Date column is the index.

After that, I made two new columns: "Tommorrow" column which is  the Close column just shifted (-1 shift) and "Target" column whose value is 1 if the price went up and 0 if the  price went down.

I used the other columns (Close, Open, Volume, High, Low) as predictors.

The split method is the same as in the other project. (train first x-100 row; test  last 100 row)


.
.
