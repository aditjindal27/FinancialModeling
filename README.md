# Financial Modeling using Differential Equations

_Adit Jindal, Stefan Quaadgras, Zhichao Wang, Nipun Chhajed_

## Description
Our project involves modeling the stocks from the S&P 500 of the New York Stock Exchange using differential equation simulations. While prior works have explored differential equation modeling of financial assets before, most publications have focused on theoretical or smaller markets with lower degrees of accuracy. Our dataset consists of the closing prices of each S\&P 500 stock for every trading day in 2022. We then simulate an ODE model and apply three different numerical methods to simulate each stock’s closing price using past closing prices for December 1st, 2022. We also simulate a stochastic differential equation model (SDE) using the same three numerical methods. A comparison of the relative errors of the six models (3 ODE and 3 SDE) is then conducted with a simple linear regression (LR) model as the baseline, and the actual price of the stock on 1st December as the truth value. We found that the chosen ODE model and the SDE model can be extended to produce relatively accurate predictions for individual stocks as well as an equally weighted portfolio of the S\&P 500 stocks. Further, higher-order numerical methods on average continually improved the predictions' accuracy. In doing so, we gained some insights into which numerical methods work best on time series of such scale and variance.

## Execution

To run an simulation, go to the appropriately named folder on the repository and download the ipynb file. Either create a jupyter notebook enviornemnt or upload it to Google Colab. The required files needed for each simulation to run is only the prices_S&P.csv. Each notebook as comments to guide you through the steps as well as graphs to better understand the results. Results.ipynb consists of a comparative analysis between the models. To run that file, you will need to add all the trained pickle files from the Trained Models folder.

## Results

The below result shows the price prediction of AAPL stock for 12/1/2022:

<img width="463" alt="Screenshot 2023-05-16 at 7 48 48 AM" src="https://github.com/aditjindal27/FinancialModeling/assets/54547947/3ee283ab-a71e-4c12-8e5b-6fd73c96c8ca">

Here, is the average error of S&P 500 which is decreasing with higher order SDE models being used.

<img width="613" alt="Screenshot 2023-05-16 at 7 49 00 AM" src="https://github.com/aditjindal27/FinancialModeling/assets/54547947/364b536d-c918-4614-8302-23b1b6495a93">
