# 🚴 London Bike Ride Dashboard

An interactive Tableau dashboard analysing London bike-sharing ride patterns, exploring how weather conditions, time of day, season, and holidays influence rider behaviour.

---

## 📁 File Information

| Property | Details |
|---|---|
| **File Name** | `London_Bike_Ride_Dashboard.twbx` |
| **File Type** | Tableau Packaged Workbook (.twbx) |
| **Tool Required** | Tableau Desktop or Tableau Public |
| **Data Source** | london_bikes_final |

---

## 📊 Dashboard Overview

The workbook contains **1 main dashboard** built from **5 individual worksheets**:

### Worksheets

| Sheet Name | Description |
|---|---|
| **Total Rides** | High-level KPI showing the overall count of bike rides across the dataset |
| **Moving Average** | Trend line of bike rides over time with a configurable moving average window to smooth short-term fluctuations |
| **Hour Chart** | Breakdown of ride counts by hour of the day, revealing peak usage periods |
| **Heat Map** | Two-dimensional heatmap showing ride density patterns across time and conditions |
| **Weather** | Analysis of how weather conditions affect the number of rides |

---

## 🗂️ Data Fields

### Core Measures & Dimensions

| Field | Description |
|---|---|
| **Count** | Number of bike rides recorded |
| **Time** | Timestamp of the ride |
| **Temp Real C** | Actual temperature in Celsius |
| **Temp Feel C** | Perceived/feels-like temperature in Celsius |
| **Humidity Percent** | Relative humidity as a percentage |
| **Wind Kph** | Wind speed in kilometres per hour |
| **Weather** | Weather condition category (e.g. clear, cloudy, rain) |
| **Season** | Season during which the ride took place |
| **Is Holiday** | Flag indicating if the ride occurred on a public holiday |
| **Is Weekend** | Flag indicating if the ride occurred on a weekend |

### Calculated Fields

| Field | Description |
|---|---|
| **Moving Average Rides** | Rolling average of ride counts using a configurable window |
| **Moving Average** | Date truncated to the selected period for trend grouping |
| **In Range** | Flags whether a data point falls within the selected date range |
| **Min Month / Max Month** | Dynamic start and end dates of the selected range |

### Interactive Parameters

| Parameter | Description |
|---|---|
| **Moving Average Period** | Sets the time granularity (day, week, month) for the moving average |
| **Moving Average Duration** | Sets the window size (default: 20 periods) for the rolling average |

---

## 🚀 How to Open

1. Download and install **[Tableau Public](https://public.tableau.com/en-us/s/download)** (free) or **Tableau Desktop**.
2. Open `London_Bike_Ride_Dashboard.twbx` directly in Tableau.
3. Navigate to **Dashboard 1** to view the full interactive dashboard.
4. Use the **Moving Average Period** and **Moving Average Duration** parameter controls to customise the trend line.
5. Explore individual worksheets for deeper analysis of specific dimensions.

---

## 🎛️ Interactive Features

- **Adjustable Moving Average** — Change the period (day/week/month) and window duration to explore different trend granularities.
- **Date Range Selection** — Filter the moving average chart to zoom into specific time periods using the dynamic range set.
- **Cross-sheet Filtering** — Clicking on chart elements filters related views across the dashboard.

---

## 💡 Use Cases

- Understanding peak bike usage hours and days in London
- Exploring the impact of weather, temperature, and wind on cycling habits
- Identifying seasonal trends in bike-share demand
- Comparing weekday vs. weekend and holiday vs. non-holiday ride patterns
- Presenting data-driven insights for urban transport or sustainability planning

---

## 📌 Notes

- This workbook uses a packaged format (`.twbx`), so all data is embedded — no external database connection is required.
- The dataset originates from London's bike-sharing system and includes environmental and temporal metadata for each ride period.
- All charts are interactive; hover over data points for tooltips and use parameter controls to customise your view.
