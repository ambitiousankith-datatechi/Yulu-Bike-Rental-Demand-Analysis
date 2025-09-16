# 🚲 Yulu Bike Rental Demand Analysis

## 📌 Project Overview
This project analyzes bike rental demand for **Yulu Bikes**, focusing on how **seasonality, weather, and environmental factors** affect user behavior.  
Using hypothesis testing and regression models, the study identifies statistically significant predictors of demand and evaluates their explanatory power.

---

## 🛠️ Tech Stack & Tools
- **Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Scikit-learn  
- **Methods**:  
  - Hypothesis Testing: t-test, ANOVA, Chi-square  
  - Regression Analysis: Simple & Multiple Linear Regression  
  - Exploratory Data Analysis (EDA)  

---

## 📂 Dataset
- Rows: ~17K daily/hourly rental events  
- Key Columns:  
  - `datetime` → timestamp of rentals  
  - `season` → Spring, Summer, Fall, Winter  
  - `weather` → Clear, Mist/Cloudy, Light Rain, Heavy Rain/Snow  
  - `atemp` → estimated temperature  
  - `humidity`, `windspeed` → weather conditions  
  - `count` → total number of rentals  

---

## 🔍 Key Findings

### ✅ Data Quality
- No missing values or duplicate rows.  
- Data types appropriate for time-series and regression analysis.  

### ✅ Bivariate Analysis
- **Season & Weather** → Significant impact on rentals (higher in Summer/Fall, lower in poor weather).  
- **Temperature (atemp)** → Strongest single predictor (~15% variance explained).  
- **Humidity (~10%) & Windspeed (~1%)** → Statistically significant but weaker effects.  
- **Working Day** → No significant difference between working days and non-working days.  

### ✅ Multivariate Regression
- **Significant Predictors**: atemp, humidity, windspeed, season (Fall/Winter), weather (Mist/Cloudy).  
- **Model Performance**: R² ≈ **0.284** on test data → explains ~28% of rental demand variability.  

---

## 📊 Visualizations
- Seasonal demand distribution plots  
- Scatter plots with regression lines (atemp, humidity, windspeed vs. rentals)  
- Weather-condition vs. rentals bar charts  
- Regression model summary tables  

---

## 🚀 Conclusion
- **Seasonality and weather** are critical factors for predicting micromobility demand.  
- Temperature is the strongest continuous predictor, but weather categories and seasonal effects are also significant.  
- Current model explains ~28% of demand — external factors (pricing, holidays, promotions, traffic conditions) likely account for remaining variability.  

---

## 📎 How to Use
1. Clone the repository:
   ```bash
   https://github.com/ambitiousankith-datatechi/Yulu-Bike-Rental-Demand-Analysis.git

📬 Author

👤 Sai Ankith Avula

https://www.linkedin.com/in/avula-sai-ankith/
