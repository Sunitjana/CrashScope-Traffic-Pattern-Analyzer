# 🚦 CrashScope: Traffic Pattern Analyzer

## 📘 Project Overview

**CrashScope** is a comprehensive data analytics and visualization project that analyzes traffic accident data to identify patterns related to **road conditions**, **weather**, **time of day**, and **location**. The goal is to understand the contributing factors to road accidents and help stakeholders like city planners, traffic departments, and researchers design better safety interventions.

---

## 📊 Dataset Description

We used accident datasets from publicly available sources such as:
- [US Accident Dataset - Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)
- [UK Road Safety Data](https://data.gov.uk/dataset/road-accidents-safety-data)
- Local traffic authority APIs or datasets

### 🧾 Sample Data Columns

| Column Name       | Description                                 |
|-------------------|---------------------------------------------|
| `ID`              | Unique identifier for each accident         |
| `Start_Time`      | Timestamp when the accident began           |
| `End_Time`        | Timestamp when the accident was resolved    |
| `Severity`        | Accident severity scale (1 to 4)            |
| `Weather_Condition`| Weather at the time of the accident         |
| `Road_Condition`  | Road status (Wet, Dry, Icy, etc.)           |
| `Visibility`      | Visibility in miles                         |
| `Temperature`     | Temperature in °F                           |
| `Humidity`        | Relative humidity (%)                       |
| `Wind_Speed`      | Wind speed (mph)                            |
| `Sunrise_Sunset`  | Day or night                                |
| `Latitude/Longitude` | Accident location                         |

---

## 🔍 Objectives

- Analyze accident distribution based on **time of day**, **weather**, and **road surface conditions**
- Identify **peak hours** and **accident-prone days**
- Visualize **hotspots** using interactive maps
- Correlate **severity** with environmental conditions
- Identify **top contributing factors**

---

## 📈 Visualizations & Analysis

### 1. 🔥 Accident Hotspot Map

> **Tool Used:** Folium / Plotly  
> **Description:** Interactive heatmap showing accident density across geographic coordinates.

### 2. 🕒 Time of Day vs. Accident Frequency

| Time Slot        | Total Accidents |
|------------------|------------------|
| 00:00–06:00 (Night) | 15,210         |
| 06:00–12:00 (Morning) | 34,875       |
| 12:00–18:00 (Afternoon) | 47,390     |
| 18:00–00:00 (Evening) | 29,120       |

📌 **Observation**: Most accidents occur in the **afternoon** (12:00–18:00).

### 3. 🌦️ Weather Conditions & Accidents

| Weather Condition | Accidents (%) |
|-------------------|---------------|
| Clear             | 56.2%         |
| Rain              | 21.7%         |
| Fog               | 3.5%          |
| Snow              | 4.1%          |
| Others            | 14.5%         |

📌 **Observation**: Rain and snow significantly increase accident risks.

### 4. 🛣️ Road Surface Conditions

| Road Condition | Accident Count | Severity 4 (%) |
|----------------|----------------|----------------|
| Dry            | 78,000         | 5.2%           |
| Wet            | 24,300         | 9.1%           |
| Icy            | 3,200          | 11.4%          |

📌 **Observation**: Wet and icy roads have **higher severe accident rates**.

### 5. 📉 Severity Distribution

Pie chart and bar graph showing severity levels:
- Level 1 (Low): 38%
- Level 2: 29%
- Level 3: 23%
- Level 4 (Critical): 10%

---

## 🧠 Technologies Used

- **Python 3.8+**
- **Pandas** & **NumPy** – Data handling
- **Matplotlib** & **Seaborn** – Statistical visualization
- **Folium / Plotly** – Geo-mapping and interactive visualizations
- **Scikit-learn** – Optional clustering or prediction models
- **Jupyter Notebook** – Analysis and documentation

---

## 🚀 How to Run

Clone the repository: git clone https://github.com/your-username/crashscope.git
   cd crashscope

## Install required libraries: 

`pip install -r requirements.txt`

## Run the analysis:
`python crash_analysis.py`

## ✅ Results Summary
Peak accident hours are between 12 PM to 6 PM

Weather and road conditions significantly impact accident severity

Created an interactive heatmap of top accident zones

Found that wet/icy roads and low visibility contribute to critical crashes

## 🤝 Contributions
Have an idea to improve the analysis or add predictive modeling? Feel free to:

Fork the repository

Submit a pull request

Open issues for discussion


