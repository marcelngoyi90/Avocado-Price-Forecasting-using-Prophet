# Avocado Price Forecasting using Prophet

## Overview
This project applies **Facebook Prophet, a powerful open-source time series forecasting library, to predict avocado prices over time.  
The goal is to model historical market data and generate reliable forecasts to understand future pricing trends in the avocado market.

---

## Dataset
The dataset used in this project is **[Avocado Prices dataset](https://www.kaggle.com/neuromusic/avocado-prices)**.  
It contains information on average avocado prices and sales volume across multiple U.S. regions.

**Key Columns:**
- `Date` — Date of observation  
- `AveragePrice` — Average price of a single avocado  
- `region` — Geographical market region  
- `type` — Conventional or organic avocados  
- `Total Volume` — Total number of avocados sold  

---

##Exploratory Data Analysis (EDA)
Before modeling, the data was explored to uncover trends and patterns:
- Visualized **average price trends** over time  
- Counted the number of entries by **region** and **year**  
- Checked for **missing values** and data consistency  

These insights helped prepare the data for Prophet and provided intuition about market behavior.

---

##  Methodology
1. **Data Preprocessing**
   - Sorted data by date  
   - Selected the relevant columns (`Date`, `AveragePrice`)  
   - Renamed columns for Prophet (`ds` and `y`)  

2. **Model Building**
   - Implemented **Facebook Prophet** for time series forecasting  
   - Trained the model on historical price data  
   - Generated future predictions for a defined forecast horizon  

3. **Forecast Visualization**
   - Plotted actual vs. predicted values  
   - Visualized Prophet’s trend, weekly, and yearly seasonal components  

---

##  Results
- Prophet effectively captured the **seasonal trends** and **overall price trajectory**.  
- The model can be used to predict future avocado prices based on historical data.  
- Forecast plots clearly show cyclical patterns in the avocado market.
