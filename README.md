# Car-Price-Prediction-with-Machine-Learning
#### In this project, I trained a machine learning model that can predict the present price of a car using certain features.
---

## Table of Contents
- [About the Project](#about-the-project)
- [Dataset Features](#dataset-features)
- [Tech Stack and Libraries](#tech-stack-and-libraries)
- [Key Steps](#key-steps)
- [Key Insights from EDA](#key-insights-from-eda)
- [Conclusion and Business Impact](#conclusion-and-business-impact)

### About the Project
This project predicts the current market price of used cars based on features like brand, manufacturing year, kilometres driven, fuel type, and more. Using Random Forest Regressor, the model helps buyers and sellers estimate fair pricing for new and pre-owned vehicles.

### Dataset Features
|Feature|Description|Type|
|-------|-----------|----|
|Car Name|Brand and model of the car|Categorical|
|Year|Manufacturing year|Numerical|
|Selling Price|Previous selling price (used)|Numerical|
|Driven Kms|Total kilometers driven|Numerical|
|Fuel Type|Petrol, Diesel, CNG, etc.|Categorical|
|Selling Type|Dealer, Individual, etc.|Categorical|
|Transmission|Manual or Automatic|Categorical|
|Owner|Number of previous owners|Numerical|
|Present Price|Current market price (Target)|Numerical|

### Tech Stack and Libraries
- Python 3.7+
- Jupyter Notebook
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

### Key Steps
- ✅ Exploratory Data Analysis (EDA) – Statistical insights & visualizations
- ✅ Data Preprocessing – Handling missing values, encoding categorical data, feature scaling
- ✅ Model Training – Linear Regression and Random Forest Regressor for price prediction
- ✅ Evaluation – Performance metrics (R², MSE); Random Forest Regressor gave a better evaluation
- ✅ Prediction – Estimating present car prices

### Key Insights from EDA
- 📌 Year vs. Price: Newer cars have higher present prices.
- 📌 Fuel Type Impact: Diesel cars are generally priced higher than petrol.
- 📌 Low Mileage Effect: Cars with fewer kilometers driven have better resale value.
- 📌 Manual vs. Automatic: Automatic cars tend to have a slightly higher price.

#### Correlation Analysis
|Feature|Correlation with Present Price|
|-------|------------------------------|
|Selling Price|	0.91 (Very Strong)|
|Transmission|0.53 (Strong)|
|Driven Kms|0.38 (Moderate)|
|Year|-0.015(Negative)|

#### Model Evaluation Comparison
|Metric|Linear Regression|Random Forest Regressor|
|------|-----------------|-----------------------|
|Mean Squared Error|22.11|15.17|
|R-Squared|0.60|0.72|


### Conclusion and Business Impact
- ✔ Strongest Price Drivers: Selling price & Fuel Type.
- ✔ Mileage Matters: High kilometer readings reduce resale value.

#### Future Improvements
- Try XGBoost for better accuracy.
- Include more features like car condition, location, etc.

