# Time-Series-Analysis-And-Forecasting-Projects

A collection of time series analysis and forecasting projects developed using Python and statistical modelling techniques. The projects cover the complete forecasting workflow, including data preparation, exploratory analysis, time series decomposition, stationarity testing, autocorrelation analysis, statistical modelling, forecasting, backtesting, and model evaluation.

---

## Projects

### Project 1 - Retail Sales Analysis & Time Series Forecasting

![Project Proof](Project-1-Retail-Sales-Forecasting/assets/project-1-proof.png)

A complete retail sales analysis and time series forecasting project using **9,800 retail transaction records** covering the period from **2015 to 2018**. The transaction-level data was transformed into a monthly time series containing **48 monthly observations**, which was then analysed using statistical time series techniques and forecasting models.

#### Key Analysis

* Data cleaning and preparation
* Exploratory Data Analysis (EDA)
* Sales analysis by state
* Sales analysis by product category
* Sales analysis by sub-category
* Monthly sales aggregation
* Time series visualisation
* Time series decomposition
* Trend analysis
* Seasonal analysis
* ACF analysis
* PACF analysis
* Dickey-Fuller stationarity testing

#### Forecasting Models

The project evaluates four forecasting approaches:

| Model                        | Description                                                  |
| ---------------------------- | ------------------------------------------------------------ |
| **AR(1)**                    | Autoregressive model using one lag                           |
| **MA(1)**                    | Moving Average model using one lag                           |
| **ARIMA(0,1,1)**             | Non-seasonal ARIMA model with first-order differencing       |
| **SARIMA(2,1,0)(1,0,0)[12]** | Seasonal ARIMA model incorporating a 12-month seasonal cycle |

#### Model Performance

The models were evaluated using a **12-month backtesting period** and three forecasting metrics:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* Mean Absolute Percentage Error (MAPE)

| Model                        |      MAE ($) |     RMSE ($) | MAPE (%) |
| ---------------------------- | -----------: | -----------: | -------: |
| AR(1)                        |     23,754.9 |     31,599.9 |     39.2 |
| MA(1)                        |     23,260.7 |     31,286.8 |     37.1 |
| ARIMA(0,1,1)                 |     25,314.3 |     29,362.0 |     62.5 |
| **SARIMA(2,1,0)(1,0,0)[12]** | **15,545.6** | **18,534.1** | **35.5** |

### Best-performing model

The **SARIMA(2,1,0)(1,0,0)[12]** model achieved the lowest MAE, RMSE, and MAPE among the four tested models.

Its seasonal component allows the model to account for the recurring **12-month retail sales pattern** identified during the time series analysis.

#### Key Findings

* California recorded the highest total sales among the states analysed.
* Technology generated the highest total sales among the three major product categories.
* Monthly sales demonstrated a recurring annual seasonal pattern.
* The series showed an underlying upward trend.
* AR(1) and MA(1) provided simpler forecasting approaches but did not explicitly capture the annual seasonal cycle.
* ARIMA(0,1,1) incorporated differencing but did not explicitly model the annual seasonality.
* SARIMA provided the strongest overall forecasting performance based on the backtesting results.

#### Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Statsmodels
* Jupyter Notebook
* Google Colab

#### Project Files

📁 **[View Project 1](Project-1-Retail-Sales-Forecasting/)**

* [Project 1 README](Project-1-Retail-Sales-Forecasting/README.md)
* [Analysis Notebook](Project-1-Retail-Sales-Forecasting/itsfa4_b21_project_1.ipynb)
* [Dataset](Project-1-Retail-Sales-Forecasting/sales.csv)

---

## Skills Demonstrated

Through the projects in this repository, the following skills are demonstrated:

### Data Analysis

* Data cleaning
* Data preprocessing
* Exploratory Data Analysis
* Data aggregation
* Statistical analysis
* Data visualisation

### Time Series Analysis

* Time series decomposition
* Trend analysis
* Seasonality analysis
* Stationarity testing
* ACF
* PACF
* Dickey-Fuller testing

### Forecasting

* Autoregressive models
* Moving Average models
* ARIMA
* SARIMA
* Seasonal forecasting
* Multi-step forecasting
* Backtesting

### Model Evaluation

* MAE
* RMSE
* MAPE
* Comparative model evaluation
* Forecast performance analysis

---

## Repository Structure

```text
Time-Series-Analysis-And-Forecasting-Projects/
│
├── README.md
│
└── Project-1-Retail-Sales-Forecasting/
    │
    ├── README.md
    ├── itsfa4_b21_project_1.ipynb
    ├── sales.csv
    │
    └── assets/
        └── project-1-proof.png
```
