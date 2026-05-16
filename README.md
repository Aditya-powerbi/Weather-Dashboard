# Weather-Dashboard
# 🌤️ Power BI Weather Dashboard

A dynamic and interactive weather dashboard built with **Power BI**, providing real-time and historical weather insights through visually rich reports and data visualizations.

---

## 📋 Table of Contents

- [Project Description](#project-description)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Dashboard Sections](#dashboard-sections)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

---

## 📌 Project Description

The **Power BI Weather Dashboard** is a business intelligence solution that visualizes weather data across multiple locations. It enables users to monitor temperature trends, precipitation levels, humidity, wind speed, and other key meteorological metrics — all in one place.

Whether you're tracking local weather patterns or comparing climate data across regions, this dashboard delivers clear, actionable insights.

---

## ✨ Features

- 🌡️ Real-time and historical temperature tracking
- 🌧️ Precipitation and rainfall analysis
- 💨 Wind speed and direction visualization
- 💧 Humidity and dew point monitoring
- 📍 Multi-location weather comparison
- 📅 Date range filtering and time-series analysis
- 🗺️ Map-based geographic weather view
- 📊 KPI cards for quick snapshot metrics

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard design and report development |
| **Power Query (M)** | Data transformation and cleaning |
| **DAX** | Custom measures and calculated columns |
| **WeatherAPI.com** | Real-time, forecast & historical weather data source |
| **Excel / CSV** | Static or historical data source |

---

## 🌐 Data Source — WeatherAPI.com

This dashboard is powered by **[WeatherAPI.com](https://www.weatherapi.com/)**, a free weather data provider trusted by 850,000+ users worldwide.

### Data Available via WeatherAPI.com
| Data Type              | Details                                                 |
|------------------------|---------------------------------------------------------|
| **Real-time Weather**  | Current temperature, humidity, wind, pressure, UV index |
| **Forecast**           | 14-day daily, hourly & 15-min interval forecasts        |
| **Historical Weather** | Hourly historical data from 2010 onwards                |
| **Air Quality**        | CO, NO₂, O₃, SO₂, PM2.5, PM10, EPA & DEFRA indexes      |
| **Astronomy**          | Sunrise, sunset, moonrise, moonset, moon phase          |
| **Geolocation**        | Timezone, IP lookup, location autocomplete              |

### API Response Fields Used in Dashboard

- `temp_c` / `temp_f` — Temperature in Celsius / Fahrenheit
- `humidity` — Humidity percentage
- `wind_kph` / `wind_dir` — Wind speed and direction
- `precip_mm` — Precipitation in mm
- `feelslike_c` — Feels like temperature
- `uv` — UV index
- `condition.text` — Weather condition description
- `air_quality` — Air quality index values

---

## ⚙️ Installation & Setup

### Prerequisites

- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) installed
- Free API key from [WeatherAPI.com](https://www.weatherapi.com/signup.aspx)

### Steps

1. **Clone or download** this repository:
   ```bash
   git clone https://github.com/your-username/powerbi-weather-dashboard.git
   ```

2. **Get your API key:**
   - Sign up at [weatherapi.com/signup.aspx](https://www.weatherapi.com/signup.aspx) (free plan available)
   - Copy your API key from the dashboard

3. **Open** the `.pbix` file in Power BI Desktop.

4. **Configure the data source:**
   - Go to `Home → Transform Data → Data Source Settings`
   - Replace `YOUR_API_KEY` with your WeatherAPI.com key
   - Update the target `location` parameter (city name, lat/lon, or IP)

   Example API endpoint used:
   ```
   https://api.weatherapi.com/v1/forecast.json?key=YOUR_API_KEY&q=London&days=7&aqi=yes
   ```

5. **Refresh the data:**
   - Click `Home → Refresh` to load the latest weather data

6. **Publish** to Power BI Service (optional):
   - Click `Home → Publish` and select your workspace

---

## 🚀 Usage

1. Open the `.pbix` file in **Power BI Desktop**
2. Use the **location slicer** to select your city or region
3. Use the **date filter** to set your preferred time range
4. Hover over charts for detailed tooltips
5. Click on visuals to cross-filter other report elements

---

## 📊 Dashboard Sections

| Section                 | Description                                                           |
|-------------------------|--------------------------------------------------------|
| **Overview**            | Summary KPIs — current temp, humidity, wind, condition |
| **Temperature Trends**  | Line chart of daily/weekly/monthly temperature changes |
| **Precipitation**       | Bar chart showing rainfall/snowfall over time          |
| **Wind Analysis**       | Wind speed gauge and directional compass visual        |
| **Location Comparison** | Side-by-side comparison of multiple cities             |
| **Map View**            | Geographic heatmap of weather conditions               |

---

## 📸 Screenshots

> *(Add your dashboard screenshots here)*

```
screenshots/
├── overview.png
├── temperature-trends.png
├── map-view.png
└── location-comparison.png
```
<img width="1313" height="739" alt="Weather Dashboard" src="https://github.com/user-attachments/assets/197ecd8b-fc15-447c-90e1-da1b09e270cc" />

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---



## 👤 Author

**Aditya Shinde**

---

> ⭐ If you found this project helpful, please give it a star on GitHub!
