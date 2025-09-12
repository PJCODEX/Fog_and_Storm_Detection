# Fog and Storm Detection – Climate Risk & Disaster Management  

##  Project Overview  
This project focuses on analyzing weather conditions related to **Fog and Storm Detection**.  
It is part of the **Climate Risk and Disaster Management Domain** and extends the **Week 1 project** with advanced data cleaning, exploratory data analysis (EDA), correlation analysis, machine learning prediction, and event insights.  

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

##  Steps Performed  

1. **Data Import & Setup**  
   - Imported libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn.  
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

7. **Machine Learning – Random Forest Model**  
   - Built a **Random Forest Classifier** to predict fog and storm events.  
   - Input features: `temperature_c`, `humidity_pct`, `wind_kmh`, `visibility_km`.  
   - Target variables: `fog`, `storm`.  
   - Model evaluation with **accuracy score and confusion matrix**.  
   - Provided prediction examples for unseen weather conditions.  

---

## Files in Repository  
- `fog_storm_dataset.csv` → Original dataset.  
- `fog_storm_dataset_clean.csv` → Cleaned dataset.  
- `fog_storm_project.ipynb` → Jupyter Notebook with full analysis + ML model.  
- `README.md` → Project description and insights.  

---

## 📈 Key Insights  

- **Visibility** decreases significantly during fog events.  
- **High humidity + low temperature** → higher fog probability.  
- **Storms** are associated with stronger winds, sometimes overlapping with fog.  
- **Cross-tab results:**  
  - 83% of fog events had **no storm**.  
  - 75% of storm events occurred **without fog**.  
  - Few days recorded **both fog and storm** together.  
- **Random Forest model** successfully predicts fog and storm events with high accuracy on the dataset.  

---

# Visualizations  

**🔹 Data Distribution**  

**🔹 Outlier Detection**  

**🔹 Time-Series Trends**  

**🔹 Visibility with Fog/Storm Markers**  

**🔹 Correlation Heatmap**  

**🔹 Pairplot – Fog**  

**🔹 Pairplot – Storm**  

**🔹 Fog vs Storm Events**  

**🔹 ML Model Performance (Confusion Matrix & Predictions)**  

---

##  Expected Outcome  
By completing this project, we learn how to:  
- Clean and preprocess weather datasets.  
- Perform **EDA and visualization** for climate-related events.  
- Analyze the relationship between **fog and storm** occurrences.  
- Build a **machine learning model** to predict weather events.  
- Draw insights relevant for **climate risk & disaster management**.  

---

##  How to Run  
1. Clone this repository.  
2. Open `fog_storm_project.ipynb` in Jupyter Notebook / Jupyter Lab.  
3. Run all cells to reproduce the analysis and visualizations.  
4. Run the **Random Forest model** section for predictions.  

---

##  Relevance to Climate Risk & Disaster Management  
- **Fog** → causes reduced visibility, transportation delays, and accidents.  
- **Storms** → cause infrastructure damage, flooding, and high-risk events.  
- **Machine learning predictions** support **early warning systems** and **policy planning** for transportation, aviation, and rural safety.  

---

✨ Built with **Python, Pandas, Matplotlib, Seaborn, Scikit-learn**  
