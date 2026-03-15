# ⚡ Energy Consumption Time Series Forecasting

## 📌 Project Overview

Energy demand forecasting is an important task for improving energy efficiency and planning electricity usage. This project focuses on forecasting short-term household energy consumption using historical time-series data.

The dataset contains electricity consumption measurements recorded over time. By analyzing temporal patterns and engineering time-based features, we build forecasting models that predict future household energy usage.

Three models were implemented and compared in this project: **ARIMA, Prophet, and XGBoost**.

---

## 🎯 Objective

The main objective of this project is to:

* Forecast short-term household energy consumption
* Extract useful time-based patterns from historical data
* Compare the performance of statistical and machine learning models

---

## 📂 Dataset

The dataset used in this project is:

**Household Power Consumption Dataset**

It contains measurements such as:

* Global Active Power
* Global Reactive Power
* Voltage
* Global Intensity
* Sub-metering values
* Date and Time of measurement

The dataset was processed and resampled to create a clean time series suitable for forecasting.

---

## ⚙️ Project Workflow

### 1️⃣ Data Preprocessing

* Combine **Date and Time** into a single datetime column
* Handle missing values
* Convert variables to numeric format

### 2️⃣ Time Series Resampling

The data was resampled into **hourly energy consumption** to simplify the forecasting task.

### 3️⃣ Feature Engineering

Several time-based features were created:

* Hour of the day
* Day of the week
* Month
* Weekend indicator

These features help machine learning models capture temporal patterns in energy usage.

### 4️⃣ Model Development

Three forecasting approaches were implemented:

**ARIMA**

* Traditional statistical time series model
* Captures autocorrelation patterns in the data

**Prophet**

* Time series forecasting library developed by Meta
* Handles seasonality and trend components effectively

**XGBoost**

* Machine learning model using engineered time features
* Captures nonlinear relationships in the data

### 5️⃣ Model Evaluation

Models were evaluated using:

* **Mean Absolute Error (MAE)**
* Comparison of predicted vs actual energy consumption

### 6️⃣ Visualization

Forecast results were visualized using:

* Time series plots
* Actual vs predicted energy consumption comparison

---

## 📊 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Statsmodels
* Prophet
* XGBoost

---

## 📁 Project Structure

```
energy-consumption-forecasting
│
├── data
│   └── household_power_consumption.csv
│
├── notebook
│   └── energy_forecasting.ipynb
│
├── images
│   └── forecast_plots.png
│
└── README.md
```

---

## 📈 Results

The models were compared based on forecasting accuracy.

Key findings:

* **ARIMA** performs well for capturing time-series dependencies
* **Prophet** models seasonal patterns effectively
* **XGBoost** benefits from engineered time-based features and often provides strong predictive performance

The comparison highlights the strengths of both statistical and machine learning approaches in energy forecasting.

---

## 🚀 Future Improvements

Possible improvements for this project include:

* Hyperparameter tuning for better model performance
* Using deep learning models such as **LSTM**
* Adding weather data to improve forecasting accuracy
* Deploying the model as a web application

---

## 📚 Learning Outcomes

Through this project, the following skills were developed:

* Time Series Data Processing
* Feature Engineering
* Forecasting Model Development
* Model Evaluation and Comparison
* Data Visualization

---

## 👨‍💻 Author

**Bilal Sarwar**

Aspiring Data Scientist passionate about applying machine learning and data analysis to solve real-world problems.

---

⭐ If you find this project useful, please consider giving it a star!
