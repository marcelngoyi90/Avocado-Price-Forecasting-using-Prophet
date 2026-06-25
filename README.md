# Avocado Price Forecasting with Prophet

A time-series project that uses Prophet to explore historical avocado-price patterns and generate future forecasts.

## Objective

The project investigates market trends, seasonality, and the future trajectory of average avocado prices across United States regions.

## Dataset

The analysis uses the [Avocado Prices dataset](https://www.kaggle.com/neuromusic/avocado-prices), including:

- `Date` — observation date;
- `AveragePrice` — average price of one avocado;
- `region` — geographic market;
- `type` — conventional or organic;
- `Total Volume` — total units sold.

## Workflow

1. Inspect data quality and visualize historical patterns.
2. Parse and aggregate the price series.
3. Rename the time and target columns to Prophet's `ds` and `y`.
4. Fit a Prophet model.
5. Generate forecasts with uncertainty intervals.
6. Inspect trend and seasonal components.

## Technology

- Python
- Pandas and NumPy
- Prophet
- Matplotlib and Plotly
- Jupyter Notebook

## Interpretation

A visually plausible forecast is not sufficient evidence of predictive quality. A production-oriented version should use time-based validation and compare Prophet with simpler baselines.

## Next steps

- report MAE, RMSE, or MAPE on a held-out time period;
- compare against naive, seasonal-naive, and ARIMA baselines;
- model regions and avocado types separately;
- document the forecast horizon and confidence intervals;
- package the model in an interactive application.
