# Water Treatment Plant Data Analysis
## Project Definition
The objective of this project is to analyze the  water treatment data for possible correlation between key parameters in attempt to predict future outcomes based on the key parameters.

## Dataset
The dataset contains daily measurements of different parameters in a water treatment plant. It has almost 4000 data points from 11 years of measurements. There are total 15+ parameters, some of the useful ones are:
-   pH: a measure of acidity or basicity of the water
-   Chlorine: a chemical used to disinfect water
-   Turbidity: a measure of the amount of suspended particles in the water
-   Hardness: a measure of the concentration of calcium and magnesium ions in the water
-  Alkalinity: a measure of the water's capacity to neutralize acids
-   Chemical dosage (alum-aluminum sulfate and lime-calcium hydroxide): the amount of chemicals added to the water during the treatment process
-   Chlorine demand: the amount of chlorine required to disinfect the water
-   UVA: ultraviolet light absorbance, a measure of the amount of UV light absorbed by the water
-   UVT: ultraviolet transmittance, a measure of the amount of UV light that passes through the water

## Research Questions
1. Can we develop a model that accurately predicts turbidity for one day in the future using historical data and various parameters such as pH, chlorine, color, turbidity, hardness, alkalinity, aluminum, temperature, and other relevant factors?
2. Can we use the predicted turbidity levels to determine the optimal chemical dosage (alum and lime) required for efficient treatment of water at the plant?
3. What is the relationship between turbidity and other water quality parameters such as chlorine demand, UVA, UVT, and color, and how do these parameters affect turbidity? Can we use this information to improve the accuracy of our turbidity prediction model?

## Models
**1. Predicting Turbidity(Time Series):** 
  - SARIMA (Seasonal Autoregressive Integrated Moving Average) can capture the seasonality of the data and make predictions based on the patterns it has learned. In our case, since we are predicting future turbidity levels, which may exhibit seasonality or other time-dependent patterns, SARIMA could be a good choice.

- STL (Seasonal and Trend decomposition using Loess) decomposition is a method for decomposing time series data into trend, seasonal, and residual components. This could be useful in understanding the patterns of turbidity and how they may be influenced by other parameters. 

**2. Predict Chemical Dosage(Regression):**

 - Linear Regression: Linear regression is a simple and widely used model that can effectively capture the linear relationship between the chemical dosage and predicted turbidity.
    
- Support Vector Regression (SVR): SVR is particularly useful when the data has a complex, nonlinear relationship. In this case, we can use SVR to model the relationship between turbidity and chemical dosage. 
