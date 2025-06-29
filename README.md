# 🌫️ AOD Time Series Analysis & Forecasting

This project focuses on time series analysis and forecasting of Aerosol Optical Depth (AOD) using data from multiple sources: MODIS Aqua, MODIS Terra, MERRA‑2 (hourly/daily), and AERONET ground-based measurements. It involves preprocessing, visualization, modeling, and 30-day forecasting using machine learning and deep learning techniques.

---

## 📊 Data Sources

- **MODIS Aqua** – Satellite-derived AOD values (monthly & daily)
- **MERRA-2** – NASA’s reanalysis data (hourly and daily)
- **AERONET Kanpur** – Ground-based AOD observations

---

## 🧹 Data Preprocessing

- **Hourly to Daily Aggregation** for MERRA-2 using resampling
- **Missing Value Handling** via interpolation
- **Outlier Detection & Treatment** using standard deviation thresholds
- **Datetime Parsing** and feature creation

---

## 🧰 Feature Engineering

- Temporal features: `year`, `month`, `day`, `day_of_year`
- Lag features: `AOD_lag_1`, `AOD_lag_3`, `AOD_lag_7`
- Rolling statistics: `rolling_mean_7`, `rolling_std_7`

---

## 📈 Visualizations

- AOD trends across different years and stations
- Monthly distribution using boxplots
- Outlier distribution
- Predicted vs Actual scatter plots
- 30-day forecasting charts

---

## 🤖 Modeling

### Machine Learning Models
- Random Forest Regressor
- MLP Regressor (Multi-layer Perceptron)

### Deep Learning
- Bidirectional LSTM using TensorFlow/Keras

### Time Series Forecasting
- ARIMA
- SARIMA

---

## 🧪 Evaluation Metrics

- **MAE** – Mean Absolute Error  
- **MSE** – Mean Squared Error  
- **RMSE** – Root Mean Squared Error  
- **R² Score** – Coefficient of Determination  

---

## 📅 Forecasting Output

- 30-day future predictions
- Comparison with ground-truth AERONET values
- Visualization in time series plots and tables

---

## 🔬 Key Insights

- Bidirectional LSTM outperforms classical models in most cases.
- MERRA-2 and MODIS Aqua show strong correlation with ground-truth.
- Outlier treatment and lag features significantly improve prediction quality.

---

## 🚧 Future Enhancements

- Include additional meteorological variables (e.g., humidity, temperature)
- Real-time web app deployment using Streamlit
- Integrate model explainability (SHAP/feature importance)
- Extend analysis to multiple Indian cities for regional comparison
