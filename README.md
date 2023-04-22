# Bachelor thesis

## Files

### Forecasting

01_ARMA-GARCH_forecasts.Rmd - ARIMA-GARCH forecasts for nearly all cases (both base case and sensitivity analysis)\
02_ARMA-GARCH_forecasts_f.Rmd - ARIMA-GARCH forecasts for rebalancing period sensitivity analysis (2-week and 3-month)\
03_HML.Rmd - estimating stock market capitalization and grouping them into 3 groups by estimated market cap\
04_ARMA-GARCH_forecasts_HML.Rmd - ARIMA-GARCH forecasts for market capitalization sensitivity analysis (high, medium and low market cap groups)\
05_XGB_forecasts.Rmd - XGBoost forecasts for nearly all cases (both base case and sensitivity analysis)\
06_XGBoost_forecasts_f.Rmd - XGBoost forecasts for rebalancing period sensitivity analysis (2-week and 3-month)\
07_XGB_forecasts_HML.Rmd - XGBoost forecasts for market capitalization sensitivity analysis (high, medium and low market cap groups)\

### Portfolio optimization

08_FMV.ipynb - optimizing portfolios for all cases, calculating equity lines and diversification metrics\

### Results

09_results.ipynb - results visualization, performance metrics calculation\

### Other important files whose names aren't self-explanatory

c_list.csv - list of constituents for the day before the first day of the period (monthly periods)\
c_list_f_05.csv - list of constituents for the day before the first day of the period (bi-weekly periods)\
df_high.xxx, df_mid.xxx, df_low.xxx - list of constituents list for the day before the first day of the period (monthly periods) for high, middle and low capitalization stocks\

price_data.xxx - adjusted close price data (for forecasting)\
price_data_close.csv - close price data (for strategy simulations)\

## Notation used in naming folders with forecasts

### Base case

arima-garch_forecasts_fixed_2_1, xgboost_forecasts - base case ARIMA-GARCH and XGBoost\

### Sensitivity analysis

...f... - rebalancing period (in months, 0.5 means 2 weeks)\
...t... - estimation window (in months)\
...H, ...M, ...L - high, middle and low capitalization\
...errdistr... - error distribution (only ARIMA-GARCH)\
...fixed_p_q - ARIMA order (only ARIMA-GARCH)\
...n... - number of lags - 1 (only XGBoost, ...n_5 - 6 lags, ...n_20 - 21 lags)\
...nrounds..., ...eta..., ...lambda..., ...max_depths..., ...subsample... - hyperparameters (only XGBoost)\
