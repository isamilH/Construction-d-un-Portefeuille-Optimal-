## Construction of an Optimal Portfolio
## Overview

This project aims to construct an optimal investment portfolio using historical price data and various mathematical and statistical methods. The goal is to maximize returns while minimizing risk, adhering to the principles of modern portfolio theory.
Table of Contents

##Project Description

1. Data Import and Preparation

    Importing Libraries: Essential libraries such as pandas, numpy, matplotlib, seaborn, and scipy.optimize are used to handle data manipulation, visualization, and optimization tasks.
    Reading Data: Historical price data is read from an Excel file named Test_PE_2023.xlsx.
    Data Cleaning: Unnecessary columns like DATE are dropped from the dataset.
    Data Description: Basic statistical descriptions of the data are generated.

2. Data Visualization

    Boxplot: A boxplot is created to visualize the distribution of the data.
    Moving Averages: The moving averages for a specified window size (e.g., 50 days) are calculated and plotted alongside historical prices to observe trends.

3. Return Calculation

    Logarithmic Returns: Logarithmic returns are calculated to understand the rate of return for each asset.
    Statistical Metrics: Mean returns and the covariance matrix of the returns are computed to capture the expected return and the risk associated with the assets.

4. Portfolio Optimization

    Objective Function: An objective function is defined to maximize the Sharpe Ratio (the ratio of portfolio return to portfolio variance).
    Constraints: A constraint function ensures that the sum of the weights of all assets in the portfolio equals one.
    Bounds and Constraints Definition: The bounds for the weights are set between 0 and 1, and constraints are added to the optimization problem.
    Optimization Process: The scipy.optimize.minimize function is used with the Sequential Least Squares Programming (SLSQP) method to find the optimal asset weights.

5. Results

    Optimal Weights: The project outputs the optimal weights for each asset in the portfolio.
    Visualization of Results: Historical prices and their moving averages are plotted to visualize the performance and trends of the assets over time.


