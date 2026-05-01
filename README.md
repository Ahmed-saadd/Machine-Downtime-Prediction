# 🏭 Manufacturing Downtime Forecasting System

## 🎯 Overview

This project builds a complete **end-to-end data pipeline** to analyze industrial machine behavior and predict **next-day downtime** using historical sensor data.

The system transforms raw machine logs into actionable insights and forecasting models to support **proactive maintenance and production planning**.

---

## 💼 Business Problem

Unplanned machine downtime leads to:

* Production delays
* Increased maintenance costs
* Reduced equipment lifespan

Most factories operate reactively — fixing machines only after failure occurs.

---

## 🚀 Solution

A **data-driven forecasting system** that:

* Analyzes historical sensor data
* Identifies failure patterns
* Predicts downtime **one day in advance**
* Provides actionable insights via dashboards

---

## 🔄 Project Pipeline

```
Raw Data → Cleaning → Aggregation → Feature Engineering → Modeling → Forecasting → Dashboard
```

---

## 📊 Dataset

* Industrial CNC machine sensor data (from Kaggle)
* Multiple machines with different operational behaviors
* Includes:

  * Pressure readings
  * Temperature signals
  * Vibration & mechanical load
  * Failure indicators

---

## 🛠️ Technologies Used

* **Python** (Pandas, NumPy, Scikit-learn)
* **SQL** (data aggregation & querying)
* **Power BI / Tableau** (dashboard visualization)
* **Jupyter Notebook** (EDA & modeling)

---

## 🔧 Data Processing

### ✔ Data Cleaning

* Removed duplicates and irrelevant columns
* Handled missing timestamps using forward fill
* Converted raw logs into structured time-series data

### ✔ Data Aggregation

* Transformed event-level data into **daily-level dataset**
* Applied:

  * Mean → sensor values
  * Max → downtime flag

### ✔ Feature Engineering

* Time-based features (day, month, etc.)
* Lag features (t-1, t-2, t-3)
* Machine-specific datasets

---

## 📈 Exploratory Data Analysis (EDA)

Key findings:

* Downtime strongly linked to:

  * Low hydraulic pressure
  * High vibration
  * Low torque
* Sensor distributions showed **distinct operating states**
* Strong correlation between mechanical stress and failures

---

## 🤖 Modeling & Forecasting

* Problem Type: **Binary Classification**
* Model: **Random Forest**
* Separate model for each machine

### 📊 Performance:

* Accuracy up to **94%**
* Reliable next-day predictions

### 📌 Example Predictions:

* Machine L1 → High risk (0.79 probability)
* Machine L2 → Stable (0.10 probability)
* Machine L3 → Moderate risk (0.25)

---

## 📊 Dashboard

Interactive dashboard includes:

* Downtime prediction KPIs
* Failure probability indicators
* Trend analysis over time
* Machine comparison heatmaps
* Feature contribution insights

---

## 📈 Key Insights

* Hydraulic pressure is the strongest failure indicator
* High vibration spikes precede downtime events
* Combined mechanical stress significantly increases risk

---

## 💡 Recommendations

* Monitor pressure and vibration daily
* Apply preventive maintenance strategies
* Adjust production load for high-risk machines
* Improve sensor data quality and logging

---

## 📁 Project Structure

```
data/           → Raw & processed datasets  
notebooks/      → EDA & modeling  
scripts/        → preprocessing & forecasting  
sql/            → queries & analysis  
dashboard/      → Power BI / Tableau files  
reports/        → insights & documentation  
```

---

## 📌 Key Value

This system enables:

* Early detection of machine failures
* Reduced downtime and costs
* Better production planning
* Data-driven decision making

---

## 🚀 Future Improvements

* Hourly-level forecasting
* Model deployment via API
* Automated retraining pipeline

---

## 👨‍💻 Author

Ahmed Saad

---

⭐ If you found this project useful, consider giving it a star!
