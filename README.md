# Indonesian Daily Weather Prediction & EDA

Exploratory Data Analysis (EDA) and Machine Learning regression pipeline to predict Indonesian daily weather temperatures using **CatBoost Regressor** and **Scikit-Learn**.

Repository: [https://github.com/raiffaza/Indonesian-Daily-Weather-Prediction-EDA](https://github.com/raiffaza/Indonesian-Daily-Weather-Prediction-EDA)

---

## Project Overview
* **Domain:** Climate & Weather Analysis (Indonesia)
* **Objective:** Clean and analyze historical meteorological data, and train a regression model to forecast daily temperature metrics.
* **Algorithm:** CatBoost Regressor
* **Evaluation Metric:** Root Mean Squared Error (RMSE)
* **Best Training RMSE:** ~0.4079

---

## Dataset
The project utilizes `idn_weather_daily.csv`, containing **303,645 records** and **14 features** across 29 Indonesian provinces[cite: 2]:
* **Geographical:** `city`, `province` (29 provinces), `island`[cite: 2]
* **Temporal:** `date` (Historical daily observations from the year 2000 onwards)[cite: 2]
* **Temperature:** `temperature_2m_max`, `temperature_2m_min`, `temperature_2m_mean`[cite: 2]
* **Precipitation & Wind:** `precipitation_sum`, `precipitation_hours`, `wind_speed_10m_max`, `wind_gusts_10m_max`[cite: 2]
* **Atmospheric:** `shortwave_radiation_sum`, `et0_fao_evapotranspiration`, `weather_code`[cite: 2]

---

## Repository Structure
```text
Indonesian-Daily-Weather-Prediction-EDA/
├── idn_weather_daily.csv.gz          # Raw daily climate dataset
├── idn_weather.ipynb               # Data cleaning, EDA, and preprocessing notebook
├── catboost_temperature_model.cbm  # Serialized trained CatBoost model
├── location_encoder.pkl            # Scikit-learn OrdinalEncoder for categorical locations
├── requirements.txt                # Environment dependencies
