## Objective

In this project, the goal is to predict the future housing market in Salt Lake City, UT, using the dataset provided by Zillow. We will also be using multiple variables (mortgage_rate, unemployment_rate, permits, and inventory) in addition to the target (HousePriceIndex to predict housing price for the next 24 months.

Incorporating real-world data from Federal Reserve Bank datasets for mortgage rate, unemployment rate and new privately-owned housing united authroized in permit-issuing places. For this portion of the analysis, Prophet model is used using historical data and external regressors like mortgage rates, permits, or unemployment to forecast future housing price.

Dataset: 
Permit: https://fred.stlouisfed.org/series/PERMIT
Unemployment Rate: https://fred.stlouisfed.org/series/UNRATE
30-Year Fixed Rate Mortgage Average: https://fred.stlouisfed.org/series/MORTGAGE30US

## Assumptions:

External variables like interest rate, CPI, etc., influence housing prices in a stable way. Without this assumption, correlation ≠ prediction

The 24-month forecast is based on patterns learned from historical trends and simulated regressors.

There are no major economic or political shocks	Pandemics, wars, etc., would break the model

We incorporate real-time mortgage rates, unemployment, housing inventory, and permit data

The model accounts for yearly seasonality but not daily or weekly trends, which are typically irrelevant for long-term housing forecasts.

Model won’t capture luxury vs. entry-level divergence unless included explicitly. 

## Approach:

Exploratory Data Analysis (EDA)

Year over year (YoY) percentage change (growth rate)

Trend-only Time Series Forecasting

Multivariate Time Series Forecasting with External Regressors

Predict Price with Upper and Lower Bound

# **Summary:**

The forecast shows Salt Lake City home prices are likely to continue rising steadily over the next 24 months, driven by stable mortgage rates, strong permitting activity, and moderate unemployment.

Forecasted Price Growth The model predicts an average compound annual growth rate (CAGR) of approximately 6%, indicating continued upward momentum in housing prices if current economic conditions persist.

Macroeconomic Sensitivity Price trends are sensitive to mortgage rates and unemployment levels. Sustained low interest rates and stable employment are likely to support further appreciation in home values.

Supply-Side Influence Building permits serve as a proxy for future housing supply. An increase in permitting activity may apply downward pressure on price growth, signaling market stabilization.

For buyers: If mortgage rates remain stable, locking in a purchase now may be more financially prudent than waiting in hopes of a price drop that the model does not project.

For investors: The relatively narrow forecast confidence intervals in the first 12 months suggest lower uncertainty in short-term price trends. This makes the market attractive for investors seeking mid-term capital gains or rental portfolio expansion.
