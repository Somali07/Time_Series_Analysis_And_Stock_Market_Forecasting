# 📊 TCS Stock Market Time Series Analysis & Dashboard

This project focuses on analyzing and forecasting the stock price movements of **Tata Consultancy Services (TCS)** using **time series analysis**. It includes feature engineering, model building (LSTM,ARIMA,SARIMA,PROPHET), visual dashboards using **Power BI**, and a Streamlit-based web dashboard.

---

## 🧾 Project Summary

- **Goal**: To understand, visualize, and forecast TCS stock performance using machine learning and interactive dashboards.
- **Tools Used**:
  - Python (Pandas, NumPy, Matplotlib, Seaborn)
  - Machine Learning (LSTM,ARIMA,SARIMA,PROPHET)
  - Power BI (for data dashboarding)
  - Streamlit (for web-based app)
  

---

## 📁 Dataset Info
TCS.NS Dataset

This dataset is locally prepared and includes the following columns:

| Column Name           | Description                        |
|-----------------------|------------------------------------|
| Tata Open             | Opening stock price                |
| Tata High             | Highest price of the day           |
| Tata Low              | Lowest price of the day            |
| Tata Close            | Closing price                      |
| Tata Adj Close        | Adjusted closing price             |
| Tata Volume           | Trading volume                     |
| Daily Return %        | Daily percentage return            |
| MA_10                 | 10-day moving average              |
| MA_30                 | 30-day moving average              |
| Volatility_10         | 10-day rolling volatility          |
| Date                  | Transaction date                   |

> ✅ Feature engineering was performed manually to derive `Daily Return %`, `MA_10`, `MA_30`, and `Volatility_10`.

---

## ⚙️ Steps Followed

### 🔍 1. Data Preprocessing
- Checked for missing values and dropped empty columns
- Removed duplicates
- Extracted `Day`, `Month`, `Year`, `Quarter` from `Date` column
- Handled scaling using MinMaxScaler
- Converted data into supervised format for model input

### 🤖 2. Model Building (LSTM,ARIMA,SARIMA,PROPHET)
- Built an LSTM,ARIMA,SARIMA,PROPHET models for price forecasting
- Trained and evaluated on TCS closing prices
- Metrics used:
  - MAE, MSE, RMSE, MAPE, R²

### 📊 3. Power BI Dashboard
- Built a report using:
  - KPI Cards (Open, Close, High, Low, Return %, Volatility)
  - Line charts for price and volume
  - Forecast vs Actual visualization

### 🖥️ 4. Streamlit Dashboard (In Progress)
- KPIs and visual charts designed
- Local dashboard working via `streamlit run app.py`
- Deployment pending final fixes

---

### ⚡ Prerequisites

Install required packages:

```bash
pip install -r requirements.txt




