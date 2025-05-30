# Power-Pulse-Household-Energy-Usage-Forecast
Data Preprocessing, Feature Engineering, Model training,Evaluation Metrics

This project aims to develop a machine learning model that predicts household energy consumption based on historical data. By accurately forecasting energy usage, the model assists consumers in monitoring their energy habits and helps energy providers optimize load management and pricing strategies.

The dataset can be dowloaded directly from the UCI Machine Learning Repository:
Download Dataset (household_power_consumption.txt)
https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption

Dataset Overview:
  1) Source: UCI Machine Learning Repository
  2) Time Period: December 2006 to November 2010 (47 months)
  3) Sampling Rate: 1-minute intervals
  4) Total Entries: 2,075,259 records
  5) Features:
            1) Date
            2) Time
            3) Global_active_power (kilowatts)
            4) Global_reactive_power (kilowatts)
            5) Voltage (volts)
            6) Global_intensity (amperes)
            7) Sub_metering_1 (watt-hours)
            8) Sub_metering_2 (watt-hours)
            9) Sub_metering_3 (watt-hours)

Objectives:
1) Predictive Modeling: Build a model to forecast global active power consumption.
2) Feature Engineering: Create meaningful features from raw data.
3) Model Evaluation: Assess various models using metrics like RMSE, MAE, and R².
4) Insights Generation: Provide actionable insights into energy usage patterns.

Approach:
1. Data Understanding and Exploration:
Load the dataset: Use pandas to read the dataset into a DataFrame.
Parse date and time: Combine Date and Time columns into a single datetime column for easier manipulation.
Initial exploration: Examine the first few rows, check for missing values, and understand the data types.

2. Data Preprocessing
Handle missing values: Identify and remove missing values as necessary.
Feature engineering:
Extract additional time-based features like hour, day, month from the datetime column.
Calculate rolling averages to capture trends.
Normalization: Scale numerical features to ensure uniformity across the dataset.

3. Model Selection and Training
Data splitting: Divide the data into training and testing sets.
Model selection:
Linear Regression
Random Forest Regressor
Gradient Boosting Regressor

4. Model Evaluation
Metrics:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R-squared (R²)

5. Comparing the metrics and selecting the best fit model

6. Visualization: Plot actual vs. predicted values to assess best fitmodel performance.

Technologies Used:
1)Programming Language: Python
2)Libraries:
    a) pandas, numpy – Data manipulation
    b) matplotlib, seaborn – Data visualization
    c) scikit-learn – Machine learning models
    d) Linearregressor,randomforestregessor,Gradient boosting Regressor – Regression modeling techniques
