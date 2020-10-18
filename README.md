# Portfolio-Planner-Budget-Analysis

In this project, we will use available APIs to obtain bank account transactions and fetch retirement portfolio prices to perform some tricky calculations and simulate the retirement investment projections. Once we have that data, we will perform a budget analysis, a retirement planning, a Monte Carlo simulation and a financial report to help build a report for customers that links to their banking and investment accounts and automatically refreshes the data and charts on login.

### Budget Analysis

In this section, we will use the Plaid API to obtain transaction and account data for the budget analysis section of the report.
1. Generate a Plaid access token to access the Developer Sandbox.
2. Use the Access token to fetch account transactions from the sandbox (We will fetch the last 90 days of transactions from the sandbox).
3. Perform basic budget analysis on the sandbox transaction and generate spending categories pie chart, spending per month bar chart and print the following:

* Last Year's Income Before Tax.

* Current Monthly Income.

* Projected Year's Income Before Tax.

### Retirement Planner

In this section, we will use the Alpaca API to fetch historical closing prices for a retirement portfolio and then run Monte Carlo simulations to project the portfolio performance at `30` years. We will then use the Monte Carlo data to answer questions about the portfolio.

#### Monte Carlo Simulation

We will create a Monte Carlo simulation for the retirement portfolio:

1. Use the Alpaca API to fetch historical closing prices for a traditional 60/40 portfolio using the `SPY` and `AGG` tickers to represent the `60%` stocks (`SPY`) and `40%` bonds (`AGG`).

2. Run a Monte Carlo Simulation of `500` runs and `30` years for the `60/40` portfolio and plot the results.

3. Select the ending cumulative returns from the Monte Carlo simulation and calculate the interval values for a `90`% confidence interval.

4. Use the ending cumulative returns, plot a histogram of the results and plot the `90%` confidence interval as vertical lines on the histogram.


#### Retirement Analysis

Use the Monte Carlo simulation data to answer the following questions:

1. What are the expected cumulative returns at `30` years for the `10th`, `50th`, and `90th` percentiles?

2. Given an initial investment of `$20,000`, what is the expected return in dollars at the `10th`, `50th`, and `90th` percentiles?

3. Given the current projected annual income from the Plaid analysis, will a `4%` withdrawal rate meet or exceed that value at the `10th` percentile? 
This is basically determining if retirement income is equivalent to current income.

4. How would a `50%` increase in the initial investment amount affect the `4%` retirement withdrawal? In other words, what happens if the initial investment had been bigger?

5. Use the Monte Carlo data and calculate the cumulative returns at the `5%`, `50%`, and `95%` quartiles and plot this data as a line chart to see how the cumulative returns change over the life of the investment.

### Financial Report

In this section, we will compile a financial report to demonstrate our calculations. 


