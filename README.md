# Multi-factor_scoring_model
Construction of a Scoring and Ranking System for Multi-Factor Quantitative Stock Selection Strategy with Daily Rebalancing: An Analysis of SSE A-shares Component Stocks

We have four main codes to reach our goal

## 1 TRC_calculation
TRC: The required data excel content and format are as follows:
There are a total 100 columns in the entire excel. For the 100 stocks with the top 100 scores on each day, we find the score data corresponding to each stock in the past thirty days. We regarded this a group, and a group is considered to have 30 rows and 100 columns. Rolling the group, the relevant calculations of TRC are used to finally obtain the capital allocation for each stock on each day.

## 2 Four-factor assignment
This code applies to the four-factor data of PEG, RSI, beta, and EI for all stocks on the SSE A-shares in the past five years. We assign different values to each factor based on its nature and economic significance and use them in subsequent scoring rankings.

## 3 Portfolio Daily Yield Matching
This code is used to match corresponding data in two excel tables. When we get the corresponding investment portfolio, we match the stock return rate based on the stock names contained in the portfolio from another excel. Then we use this data to calculate the stock portfolio simple cumulative return.

## 4 PnL_curve_drawing
The data used by this code include the cumulative simple returns of the SSE A-shares and the simple cumulative returns of the stock portfolio. We use the CSI 300 data as the baseline and draw the two sets of data in the same coordinates. The coordinate X is the corresponding time span, and Y is the corresponding simple cumulative return rate of the stock.
