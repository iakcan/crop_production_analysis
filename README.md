# Crop Production Analysis in India using Statistical Modeling

This project analyzes agricultural production data in India using statistical methods and modeling techniques to identify key environmental and soil-related factors influencing crop yield.

---

## 🚀 Project Overview

Agricultural productivity depends on complex interactions between climate conditions, soil properties, and farming practices.

This project explores crop production data across Indian states to:

- Identify patterns in agricultural output  
- Analyze the impact of rainfall, temperature, and soil nutrients  
- Build interpretable statistical models for yield prediction  

---

## 📂 Dataset

The dataset contains:

- ~100,000 observations  
- Soil nutrients, climate variables, and production metrics

👉 Dataset sample:  
[View full dataset](./data/Crop_production.csv)

---

## 🔬 Methodology

### Data Preprocessing

- Removed redundant variables  
- Outlier removal (IQR method)  
- Feature engineering (Year_Index, regions, crop categories)  

---

### Exploratory Data Analysis

### Regional Production

![Production by Region](./images/production_by_region.png)

- West region has the highest production  
- Strong regional variation in agricultural output  

---

### Climate Analysis

![Rainfall by Region](./images/rainfall_by_region.png)

![Temperature by Region](./images/temperature_by_region.png)

- Rainfall varies significantly across regions  
- Temperature differences influence productivity  

---

### Temporal Trends

![Rainfall vs Production](./images/rainfall_production_time.png)

![Temperature vs Production](./images/temperature_production_time.png)

- Increased rainfall → lower production  
- Temperature trends correlate with yield changes  

---

### Crop Type Analysis

![Crop Production](./images/crop_type_production.png)

- Food crops dominate total production  
- Spices show the lowest production levels  

---

### Correlation Analysis

![Heatmap](./images/correlation_heatmap.png)

- Strong correlation: Area ↔ Production  
- Weak correlations between climate and nutrients  

---

## 📉 Model Development

### PCA (Dimensionality Reduction)

![PCA](./images/pca_plot.png)

- 5 components explain ~77% of variance  
- Soil nutrients negatively related to pH  

---

### Model Results

- Generalized Linear Model (GLM)  
- Model selection using AIC  
- Best model includes interaction terms  

---

### Model Performance

![Model Testing](./images/model_testing.png)

- RMSE ≈ **7285.52**  
- Model captures general trends but shows variance  

---

## 🧠 Key Insights

- Climate variability strongly impacts crop production  
- Excess rainfall negatively affects yield  
- Soil nutrients interact with pH  
- Area is the strongest production driver  

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)

---

## ⚠️ Limitations

- Implicit time dimension (no explicit years)  
- High redundancy in dataset  
- Crop-specific yield differences not normalized  

---

## 🔮 Future Work

- Apply ML models (XGBoost, Random Forest)  
- Improve feature engineering  
- Integrate external climate datasets  

---

## ⚡ Implementation

The model implementation is available in the `notebooks/Crop_Production.ipynb` directory.

---

## 👩‍💻 Author

**Irem Akcan**
