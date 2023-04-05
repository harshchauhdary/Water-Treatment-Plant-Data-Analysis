# Water Treatment Plant Data Analysis - [Riipen](https://app.riipen.com/matches/EzvGnoLn)
## Project Definition
The objective of this project is to analyze the  water treatment data for possible correlation between key parameters in attempt to predict future outcomes based on the key parameters.

## Dataset
The dataset contains daily measurements of different parameters in a water treatment plant. It has almost 4000 data points from 11 years of measurements. There are total 15+ parameters, some of the useful ones are:
-   pH: a measure of acidity or basicity of the water
-   Chlorine: a chemical used to disinfect water
-   Turbidity: a measure of the amount of suspended particles in the water
-   Hardness: a measure of the concentration of calcium and magnesium ions in the water
-   Alkalinity: a measure of the water's capacity to neutralize acids
-   Chemical dosage (alum-aluminum sulfate and lime-calcium hydroxide): the amount of chemicals added to the water during the treatment process
-   Chlorine demand: the amount of chlorine required to disinfect the water
-   UVA: ultraviolet light absorbance, a measure of the amount of UV light absorbed by the water
-   UVT: ultraviolet transmittance, a measure of the amount of UV light that passes through the water

## Research Questions
1. Can we develop a model that accurately predicts turbidity for one day in the future using historical data and various parameters such as pH, chlorine, UVA, UVT, color, turbidity, hardness, alkalinity, aluminum, temperature, and other relevant factors?
2. Can we use the predicted turbidity levels to determine the optimal chemical dosage (alum and chlorine) required for efficient treatment of water at the plant?

## Models
**1. Predicting Turbidity(Time Series):** 
  - Prophet: Prophet is a time series forecasting model that can capture trends, seasonality, and other time-dependent patterns in the data. Prophet is suitable for this task as it can handle seasonal and trend changes in the data and produce accurate forecasts. Additionally, Prophet has the ability to handle missing values and outliers, which can be common in water quality data.

- STL decomposition: Seasonal and Trend decomposition using Loess(STL) decomposition is a method for decomposing time series data into trend, seasonal, and residual components. This could be useful in understanding the patterns of turbidity and how they may be influenced by other parameters. 

**2. Predict Chemical Dosage(Regression):**

 - Random Forest Regressor: Random Forest Regressor is a robust ensemble model that can handle nonlinear relationships between the input features and output variable, making it suitable for predicting optimal chemical dosages based on the turbidity.
    
- XGBoost: XGBoost is a powerful algorithm that can handle complex relationships between variables and is often used in regression problems. It can capture non-linear relationships between turbidity and chemical dosage, making it a good choice for predicting the optimal dosage. Additionally, XGBoost is highly scalable and can handle large datasets, which can be useful for our problem.
