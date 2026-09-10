# 🌾 Seasonal Agriculture Performance Analysis

## 📌 Project Overview
This project analyzes **4,000 agricultural farm records** across **3 seasons** (Kharif, Rabi, Zaid) and **8 Indian states** to uncover how agricultural performance varies seasonally. The analysis examines **28 parameters** including crop types, environmental factors, resource usage, and economic metrics to identify meaningful patterns and trends.

## 🎯 Objectives
- Compare profitability, yield, and resource usage across seasons
- Identify the most profitable crops and farming practices for each season
- Analyze how environmental factors (rainfall, temperature) impact crop yields
- Provide data-driven recommendations for farmers and agricultural planners

## ❓ Problem Statement

In the agricultural sector, maximizing profitability while efficiently using resources like water, fertilizer, and land is a critical challenge. Farmers and agribusinesses lack data-driven insights to make informed decisions about which crops to grow, which seasons to prioritize, and how to optimize resource usage. This project addresses this gap by analyzing seasonal agricultural data to provide actionable recommendations.

## 📊 Dataset
- **Records:** 4,000 farm entries
- **Features:** 28 parameters
- **Crops:** 8 types (Chilli, Cotton, Groundnut, Maize, Pulses, Rice, Sugarcane, Wheat)
- **Seasons:** Kharif, Rabi, Zaid
- **States:** Andhra Pradesh, Gujarat, Karnataka, Madhya Pradesh, Maharashtra, Punjab, Tamil Nadu, Telangana

  ## 🧹 Data Cleaning Process

1. **Data Inspection:** Used `df.info()`, `df.describe()`, and `df.shape` to understand the data structure (4,000 records × 28 columns).

2. **Missing Value Identification:**
   | Column | Missing Count | Percentage |
   |--------|---------------|------------|
   | Rainfall_mm | 48 | 1.2% |
   | Soil_Moisture_pct | 40 | 1.0% |
   | Yield_Tonnes_Ha | 32 | 0.8% |

3. **Missing Value Handling:** Imputed missing values using the **median** of each column to minimize the impact of outliers.

4. **Duplicate Check:** No duplicate records were found in the dataset.

5. **Export:** The cleaned dataset was saved as `seasonal_agriculture_cleaned.csv`.

## 🔍 Exploratory Data Analysis (EDA)

The EDA focused on:
- **Descriptive Statistics:** Mean, median, and spread of all numerical features
- **Correlation Analysis:** Relationships between environmental factors and crop yield
- **Seasonal Analysis:** Comparing profitability, yield, and resource usage across seasons
- **Crop Analysis:** Identifying the most and least profitable crops
- **Outlier Detection:** Identifying extreme values in profit and yield
- **Disease Risk Analysis:** Understanding pest/disease patterns across seasons and crops

## 🔧 Technology Stack
- **Language:** Python 3
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, SciPy
- **Platform:** Google Colab / Jupyter Notebook

---

## 📈 Key Findings

### 1. Seasonal Performance
| Season | Avg Yield (T/Ha) | Total Profit (INR) | Disease Risk (%) |
|--------|------------------|--------------------|------------------|
| **Kharif** | **2.08** (Highest) | ₹447.2M | 52.3% |
| **Rabi** | 1.82 | **₹526.8M** (Highest) | **44.8%** (Lowest) |
| **Zaid** | 1.72 | ₹298.5M | 48.6% |

### 2. Crop Insights
- **Rice** is the most common crop (17.3% of all records)
- **Chilli** is the most profitable crop across ALL seasons
- **Chilli + Drip Irrigation** = Best combination

### 3. Environmental Impact
- Rainfall helps Kharif yield (Correlation: +0.42)
- Temperature helps Zaid yield (Correlation: +0.41)
- Sunlight benefits ALL seasons (+0.15 to +0.33)

---

## 📊 Visualizations

### 1. Seasonal Performance Dashboard
*4-in-1 view of profit, yield, crop-profit, and resource usage*

<img width="1207" height="573" alt="profit vs season " src="https://github.com/user-attachments/assets/a8e8d82a-dab2-4bc8-9560-5e7a37bb8e97" />


**What it shows:**
- **Top Left:** Total Profit by Season (Rabi highest at ₹526.8M)
- **Top Right:** Yield & Profit per Hectare
- **Bottom Left:** Profit Heatmap - Crops vs Seasons (Chilli dominates)
- **Bottom Right:** Resource Usage by Season (Water & Fertilizer)

---

### 2. Correlation Heatmaps
*Environmental factors vs yield by season*

<img width="1522" height="593" alt="Screenshot 2026-09-09 093529" src="https://github.com/user-attachments/assets/d57fdf5d-307b-42e0-a199-6990b219f8b1" />

**Key Insights:**
- **Kharif:** Rainfall helps (+0.42), Temperature hurts (-0.38)
- **Rabi:** Moderate correlations, balanced conditions
- **Zaid:** Temperature helps (+0.41), Rainfall hurts (-0.35)

---


### 3. Disease Risk Analysis
*Risk patterns across seasons and crops*

<img width="568" height="442" alt="Screenshot 2026-09-09 094018" src="https://github.com/user-attachments/assets/34a9fa5f-1afe-448a-a6fa-c2b385a7e0c7" />

**Key Insights:**
- **Kharif** has highest disease risk (52.3%)
- **Rabi** has lowest disease risk (44.8%)
- **Sugarcane** highest risk (56.7%), **Maize** lowest (46.3%)
---
## 📊 Power BI Dashboard

<img width="1491" height="860" alt="Screenshot 2026-09-10 075423" src="https://github.com/user-attachments/assets/2b47d924-9828-4900-bcbf-c1dd7f251a03" />


### Dashboard Features:
- **3 KPI Cards:** Total Profit, Average Yield, Total Records
- **4 Visualizations:** 
  - Profit by Season
  - Profit by Crop
  - Yield by Irrigation
  - Crop-Season Profit Heatmap
- **Interactive Filters:** Season, State, Crop Type

### Key Dashboard Insights:
1. Rabi season generates highest profit (₹526.8M)
2. Chilli is the most profitable crop
3. Drip irrigation gives best yield
4. Crop performance varies significantly by season

---

## 💡 Recommendations
✅ **Farmers:** Prioritize Chilli + Drip Irrigation for maximum profit|
✅ **Planners:** Promote Rabi season for higher profitability |
✅ **Policymakers:** Support water conservation in Kharif, optimize fertilizer in Zaid |
✅ **All:** Implement pest management during high-risk seasons

---

## 🚀 Future Scope
- AI-powered crop recommendation system
- IoT sensors for real-time farm monitoring
- Mobile app for farmers
- Climate change impact assessment
- National agricultural data platform

---
## ✅ Conclusion

This project successfully analyzed 4,000 agricultural records to identify key patterns in seasonal profitability, crop performance, and resource efficiency. The findings reveal that the **Rabi season generates the highest total profit (₹526.8M)** , **Chilli is the most profitable crop**, and **Drip irrigation delivers the best yield efficiency**. These insights provide a clear, data-driven roadmap for farmers, planners, and policymakers to make informed decisions that enhance agricultural profitability and sustainability.

---
## 📁 Repository Contents

| File | Description |
|------|-------------|
| `seasonal_agriculture.csv` | Original dataset |
| `seasonal_agriculture_cleaned.csv` | Cleaned dataset |
| `seasonal_agriculture.ipynb` | Jupyter Notebook with EDA |
| `Seasonal Agricultural Performance Analysis.pptx` | Project presentation |
| `Seasonal_Agriculture_Dashboard.pbix` | Power BI Dashboard file |
| `README.md` | Project documentation |
