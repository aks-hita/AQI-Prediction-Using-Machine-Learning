# AQI-Prediction-Using-Machine-Learning
This project aims to develop and evaluate supervised regression models for predicting the Air Quality Index (AQI) using air pollutant and meteorological data, with the ultimate goal of contributing to early warning systems.
Objective:

To develop a supervised regression model that predicts AQI using air pollutants and meteorological data for early warning systems.
Data Used:

The project uses the city_day.csv dataset, containing daily air quality and meteorological measurements from Indian cities. It includes features like PM2.5, PM10, NO, NO2, CO, O3, Benzene, Toluene, Xylene, AQI, City, and Date. Data from January 1, 2019, onwards is used, with a subset of 4000 samples for demonstration.
Methodology:

The project follows a standard machine learning workflow:

    Data Loading and Preprocessing: Load data, convert 'Date' to datetime, filter for recent entries, sample the data, handle missing 'PM2.5' and 'PM10' values using median imputation, and treat outliers using IQR.
    Feature Engineering: Extract 'Month' from 'Date' and label encode the 'City' column.
    Feature Selection: Select key features like 'PM2.5', 'PM10', 'NO2', 'CO', 'O3', 'Month', and 'City'.
    Data Scaling: Scale features using StandardScaler.
    Model Training: Train Linear Regression, Decision Tree Regressor, and Random Forest Regressor.
    Model Evaluation: Evaluate models using R-squared (R2) and Root Mean Squared Error (RMSE), and visualize performance.
    Feature Importance: Analyze and visualize feature importance for the best model (Random Forest).
    Early Warning Simulation: Demonstrate AQI prediction and categorization for early warnings.

How to Use:

Execute the notebook cells sequentially. This involves data loading, cleaning, preprocessing, model training, evaluation, and visu
