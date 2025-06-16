# 🌞 Solar Irradiance Prediction Using Satellite Data and Machine Learning.

![Preview](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Gaurav_Lute_MT2313poster.pdf)

## 🔍 Overview

This project aims to predict **Global Horizontal Irradiance (GHI)** — a crucial measure for solar energy planning — using advanced **Machine Learning** and **Time Series Forecasting** techniques. Using a decade’s worth of satellite data from **NASA POWER**, we model both short-term and seasonal solar patterns for Pune, India.

> 🎯 **Goal:** Build and evaluate predictive models that can assist in solar energy management, smart grid integration, and sustainable planning.

---

## 📌 Project Objectives

### ✅ Objective 1: ML-based GHI Prediction  
Build machine learning models to predict daily GHI values using environmental features.

### ✅ Objective 2: GHI Forecasting for March 2025  
Use time series models to forecast future GHI values — targeting March 2025.

---

## 🛰️ Dataset Description

- **Source:** NASA POWER API  
- **Location:** Pune, India (Lat: 18.52°N, Lon: 73.86°E)  
- **Duration:** Feb 2016 – Feb 2025  
- **Resolution:** Daily  
- **Target:** `ALLSKY_SFC_SW_DWN` (Global Horizontal Irradiance)  
- **Features:** T2M, RH2M, WS10M, Precipitation, Cloud Cover, Pressure, DOY, Lag values

📊 ![Dataset Overview](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/Dataset_description.png)

---

## 🔧 Methodology

📂 Our modeling pipeline includes:
- Exploratory Data Analysis (EDA)
- Feature Engineering (lag values, rolling averages, cyclic encoding)
- Model development and evaluation
- Forecast visualization

📈 ![Workflow](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/Flow%20Chart.png)

---
## 🔧 Key Insights
📈 ![Workflow](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/EDA.png)

## 🛰️Access Report
![Report](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/EDA.png)

## 🤖 Models Used

### ML Models (Objective 1)
- Random Forest  
- Gradient Boosting  

### Time Series Models (Objective 2)
- XGBoost  
- LightGBM  
- ARIMA  
- Prophet  

---

## 📈 Results Snapshot

### 🧠 ML Models (Daily Prediction)

| Model            | MSE   | R² Score |
|------------------|-------|----------|
| Random Forest    | 0.39  | 0.98     |
| Gradient Boosting| 0.43  | 0.98     |

### 🔮 Forecasting Models (March 2025)

| Model      | RMSE / MAPE | R² Score |
|------------|-------------|----------|
| XGBoost    | 0.192 (RMSE)| 0.891    |
| LightGBM   | 0.050 (RMSE)| 0.856    |
| ARIMA      | 0.035 (RMSE)| —        |
| Prophet    | 0.03 (MAPE) | —        |

---

## 🖼️ Visual Results

### 📅 March 2025 Forecast Comparison

| Model        | 1-Month Prediction | 3-Month Prediction |
|--------------|--------------------|---------------------|
| **XGBoost**  | ![XGBoost March](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/Xgboost_march.png) | ![XGBoost 3-month](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/xgboost_three.png) |
| **LightGBM** | ![LGBM March](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/Lightgbm_one.png) | ![LGBM 3-month](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/Lightgbm_three.png) |
| **Prophet**  | ![Prophet March](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/prophet_one.png)| ![Prophet 3-month](https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning./blob/main/Plots/prophet_three.png) |

---

## 📝 Conclusion

- XGBoost gave the most **accurate** and **stable** forecasts across both objectives.
- Prophet effectively captured **seasonality**, while ARIMA offered the **lowest RMSE**.
- Feature engineering was crucial — particularly lag values and cyclic transformations.

---

## 🚀 Future Work

- Integrate deep learning models (e.g., LSTM, TCN)
- Deploy live forecasting dashboard using Streamlit or Flask
- Extend analysis across multiple cities for grid-scale energy forecasting

---

## 📁 Repository Structure


---

## 👤 Author

**Gaurav Prakash Lute**  
M.Tech – Modeling and Simulation  
Savitribai Phule Pune University  
📧 lute.gaurav@scms.unipune.ac.in  📧 lutegaurav1@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/gauravlute01)

---

## 📌 Citation

```bibtex
@project{lute2025solar,
  title     = {Solar Irradiance Prediction Using Satellite Data and Machine Learning},
  author    = {Gaurav Prakash Lute},
  year      = {2025},
  institution = {Savitribai Phule Pune University},
  url       = {https://github.com/gauravlute01/Solar-irradiance-Prediction-Using-Satellite-Data-and-Machine-Learning}
}
