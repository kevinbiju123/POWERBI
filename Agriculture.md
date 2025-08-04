# 🌧️ Rainfall Analysis Dashboard – Power BI Project

This repository contains an interactive Power BI dashboard that analyzes average rainfall data across years, seasons, crops, and locations. It uses agricultural rainfall data to help stakeholders such as farmers, policymakers, and agronomists make informed decisions about crop selection and regional planning based on rainfall patterns.

---

## 🧩 Problem Statement

Rainfall is one of the most crucial factors affecting agricultural productivity in India, especially in monsoon-dependent regions. However, decisions around cropping, irrigation, and risk mitigation are often made without structured insights into rainfall distribution. This project aims to centralize and visualize rainfall data to uncover patterns by time, crop type, and location, enabling better resource planning, policy design, and support for climate-resilient agriculture.

---

## 📂 Dataset Used

| File Name          | Description                                                      |
|--------------------|------------------------------------------------------------------|
| `Agriculture.xlsx` | Contains historical rainfall data categorized by year, season, crop, and location. |

---

## ⚙️ Steps Followed

1. **Data Preparation**
   - Loaded and cleaned data from `Agriculture.xlsx`.
   - Converted fields into usable formats for time series, categorical analysis, and aggregation.
   - Derived average rainfall metrics using DAX measures in Power BI.

2. **Visualization Design**
   - Applied consistent theme (pink palette) for styling and visual clarity.
   - Organized data into four key insights panels:
     - Rainfall by Year
     - Rainfall by Season
     - Rainfall by Crop
     - Rainfall by Location

3. **Filtering and Interactivity**
   - Enabled slicers for user-driven analysis by filters such as crop type or year.
   - Applied tooltips and data labels for clear interpretation.

---

## 📊 Dashboard Highlights

### 1. **Average Rainfall by Year**
   - Displays yearly rainfall from 2005 to 2020.
   - Peak observed near 2008 and 2010 (~2900+ mm), while 2020 showed a drop (~2491 mm).

### 2. **Rainfall by Season**
   - Rabi: 2823 mm  
   - Kharif: 2816 mm  
   - Zaid: 2791 mm  
   Insight: Rabi season had slightly higher average rainfall across regions.

### 3. **Rainfall by Crops**
   - Top crops by average rainfall:
     - **Paddy:** 3139 mm
     - **Arecanut:** 3013 mm
     - **Cardamom:** 2984 mm
   - Crops like **Tea**, **Coffee**, and **Ginger** also showed significant rainfall needs.

### 4. **Rainfall by Location**
   - **Bangalore** recorded the highest average rainfall (3.5K mm).
   - Other high-rainfall regions: **Raichur**, **Kasaragod**, **Mangalore** (~2.9K mm each).
   - Locations like **Kodagu** and **Davangere** had relatively lower averages (~2.7K mm).

---

## ✅ Conclusions

- Rainfall distribution varies moderately across seasons but shows greater variation across years and crops.
- Some crops (e.g., Paddy, Arecanut) demand higher rainfall and are best suited for high-rain regions like Bangalore and Mangalore.
- Decision-makers can use these insights to align crop planning with historical rainfall trends.

---

## 🔄 Future Enhancements

- Integrate soil moisture and yield data for correlation with rainfall.
- Add predictive modeling for future rainfall trends.
- Include irrigation dependency for drought-prone regions.

---

## 📎 License

This dashboard and dataset are intended for educational and non-commercial use. Attribution to the original data source is recommended where applicable.

