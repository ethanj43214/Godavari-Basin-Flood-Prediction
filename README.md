# Godavari Basin Flood Prediction & Hydrological Analysis

A data science project focused on flood prediction in the Godavari river basin 
using multi-source hydrological and meteorological data collected across 15 stations.

---

## 🎯 Objective

Built a flood prediction model for the Godavari Basin by integrating data from 
multiple sources and exploring deep learning approaches (LSTM & GRU).

---

## 📍 Study Area

- **Basin**: Godavari River Basin
- **Stations**: 15 stations across Maharashtra, Telangana & Andhra Pradesh
- **Tributaries**: Adhala, Indravati, Machkund, Maner, Peddavagu, Pamuleru, Wardha
- **Date Range**: 01 June 2018 – 30 September 2025

---

## 📊 Dataset — 12 Parameters

| # | Parameter | Source |
|---|-----------|--------|
| 1 | River Water Discharge | WRIS (indiawris.com) |
| 2 | River Water Level | WRIS (indiawris.com) |
| 3 | Temperature at 2 Meters | NASA POWER (DAV) |
| 4 | Relative Humidity at 2 Meters | NASA POWER (DAV) |
| 5 | Surface Pressure | NASA POWER (DAV) |
| 6 | Wind Speed at 2 Meters | NASA POWER (DAV) |
| 7 | Surface Soil Wetness | NASA POWER (DAV) |
| 8 | Root Zone Soil Wetness | NASA POWER (DAV) |
| 9 | Profile Soil Moisture | NASA POWER (DAV) |
| 10 | Rainfall | IMDLib |
| 11 | Minimum Temperature (tmin) | IMDLib |
| 12 | Maximum Temperature (tmax) | IMDLib |

---

## 🛠️ Tools & Technologies

- **Python** — Data extraction, cleaning, and merging
- **imdlib** — IMD gridded data extraction
- **NASA POWER DAV** — Meteorological data
- **Pandas, NumPy** — Data processing
- **TensorFlow / Keras** — LSTM & GRU model training
- **Google Colab** — Development environment

---

## 🔧 Steps Performed

### 1. Data Collection
- Extracted rainfall, tmin, tmax for 15 stations using IMDLib
- Downloaded meteorological parameters from NASA POWER Data Access Viewer
- Collected river discharge and water level data from WRIS

### 2. Data Cleaning & Merging
- Removed missing values and handled -999.0 IMD fill values
- Filtered data to common date range: 01 June 2018 – 30 September 2025
- Merged IMD and NASA datasets on Year, Day of Year, and Station ID
- Structured final dataset with all 12 parameters vertically stacked by station

### 3. Prediction Modelling
- Explored LSTM and GRU deep learning models for flood prediction
- Used time-series sequences of all 12 parameters as input features

---

## 💡 Key Highlights

- Integrated 3 data sources into a single clean dataset
- Covered 15 hydrological stations across 3 states
- Dataset spans 7 monsoon seasons (2018–2025)
- Applied deep learning methods for time-series flood prediction

---

Built with ❤️ using Python | IMDLib | NASA POWER | WRIS
