# Fog and Storm Detection – Climate Risk & Disaster Management  

##  Project Overview  
This project focuses on analyzing weather conditions related to **Fog and Storm Detection**.  
It is part of the **Climate Risk and Disaster Management Domain** and extends the **Week 1 project** with advanced data cleaning, exploratory data analysis (EDA), correlation analysis, and event insights.  

The goal is to understand how atmospheric conditions (temperature, humidity, wind, visibility) influence fog and storm formation, and how these insights can contribute to **climate risk assessment and disaster management**.  

---

## 📊 Dataset  
The dataset (`fog_storm_dataset.csv`) contains **daily weather observations** with the following columns:  

- `date` → Observation date  
- `temperature_c` → Temperature in °C  
- `humidity_pct` → Relative humidity (%)  
- `wind_kmh` → Wind speed (km/h)  
- `visibility_km` → Visibility distance (km)  
- `fog` → Fog event (1 = Yes, 0 = No)  
- `storm` → Storm event (1 = Yes, 0 = No)  

 Dataset Size: **10 rows × 7 columns**  

---

## 🛠 Steps Performed  

1. **Data Import & Setup**  
   - Imported libraries: Pandas, NumPy, Matplotlib, Seaborn.  
   - Loaded dataset and standardized column names.  

2. **Data Cleaning**  
   - Converted columns to correct datatypes.  
   - Removed duplicates.  
   - Handled missing values with interpolation.  

3. **Feature Engineering**  
   - Extracted new time features: `year`, `month`, `day`, `week`, `dayofweek`, `dayofyear`.  

4. **Exploratory Data Analysis (EDA)**  
   - Distribution plots (histograms + KDE).  
   - Boxplots to detect outliers.  
   - Time-series visualization of weather variables.  
   - Markers for fog and storm events.  

5. **Correlation Analysis**  
   - Pearson & Spearman correlation heatmaps.  
   - Pairplots for visualizing relationships with fog/storm.  

6. **Event Relationship Analysis**  
   - Cross-tabulation of fog vs storm occurrences.  
   - Stacked bar charts for co-occurrence patterns.  

---

## 📂 Files in Repository  
- `fog_storm_dataset.csv` → Original dataset.  
- `fog_storm_dataset_clean.csv` → Cleaned dataset.  
- `fog_storm_project.ipynb` → Jupyter Notebook with full analysis.  
- `README.md` → Project description and insights.  
- `/images` → Folder containing saved plots.  

---

## 📈 Key Insights  

- **Visibility** decreases significantly during fog events.  
- **High humidity + low temperature** → higher fog probability.  
- **Storms** are associated with stronger winds, sometimes overlapping with fog.  
- **Cross-tab results:**  
  - 83% of fog events had **no storm**.  
  - 75% of storm events occurred **without fog**.  
  - Few days recorded **both fog and storm** together.  

---

## Visualizations  

### 🔹 Data Distribution  
![Histogram KDE](images/distributions.png)  

### 🔹 Outlier Detection  
![Boxplot](images/boxplot.png)  

### 🔹 Time-Series Trends  
![Time Series](images/timeseries.png)  

### 🔹 Visibility with Fog/Storm Markers  
![Visibility](images/visibility_fog_storm.png)  

### 🔹 Correlation Heatmap  
![Correlation Heatmap](images/correlation.png)  

### 🔹 Pairplot – Fog  
![Pairplot Fog](images/pairplot_fog.png)  

### 🔹 Pairplot – Storm  
![Pairplot Storm](images/pairplot_storm.png)  

### 🔹 Fog vs Storm Events  
![Fog Storm Bar](images/fog_storm_bar.png)  

---

##  Expected Outcome  
By completing this project, we learn how to:  
- Clean and preprocess weather datasets.  
- Perform **EDA and visualization** for climate-related events.  
- Analyze the relationship between **fog and storm** occurrences.  
- Draw insights relevant for **climate risk & disaster management**.  

---

##  How to Run  
1. Clone this repository.  
2. Open `fog_storm_project.ipynb` in Jupyter Notebook / Jupyter Lab.  
3. Run all cells to reproduce the analysis and visualizations.  

---

##  Relevance to Climate Risk & Disaster Management  
- **Fog** → causes reduced visibility, transportation delays, and accidents.  
- **Storms** → cause infrastructure damage, flooding, and high-risk events.  
- **Overlap analysis** supports **early warning systems** and **policy planning** for transportation, aviation, and rural safety.  

---

##  Future Improvements  
- Extend dataset with **long-term weather records**.  
- Use **machine learning models** to predict fog/storm events.  
- Integrate **real-time weather APIs** for live monitoring.  
- Build an **interactive dashboard** for decision-makers.  

---

✨ Built with **Python, Pandas, Matplotlib, Seaborn**  
