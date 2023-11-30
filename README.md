# Environmental Data Analysis Project

## Overview:

This repository focuses on predicting healthy and unhealthy days' percentages in North Carolina by leveraging machine learning techniques. The project entails preprocessing and analyzing environmental data to gain insights into air quality trends. 

## Project Description:

The primary objective is to employ Linear Regression, facilitated by Scikit-learn, for predicting air quality metrics. The dataset, spanning from 1980 to 2023, includes comprehensive environmental information. Key tasks involve preprocessing and transforming the data to build a robust predictive model.

## Preprocessing Steps:

1. **Data Cleaning:** Address missing values and handle outliers to ensure data integrity.
2. **Data Transformation:**  Certain columns are converted to more efficient data types.
3. **Feature Engineering:** Derive meaningful features such as the Unhealthy Days percentage from raw data.
4. **2023 Data:** Finding Data for Mecklenburg and Wake county in order to fit into our model
   Files: meck_co.ipynb , merge-csv.ipynb , nc_2023_data.ipynb, and updated_analysis_notebook.ipynb

## Data Storage in SQL:

1. **Database Storage:** Data is saved in table format, suitable for complex queries and analysis.
2. **Data Migration:** Transfer the preprocessed data into the SQL database for efficient storage and retrieval.
   Files: nc_aqi_data.db and updated_database.ipynb 
   
## Linear Regression Model: 
1. **Target Variable Definition:** Clearly define the target variable - unhealthy days' percentages.
2. **Model Selection:** Choose Linear Regression for predicting air quality metrics.
3. **Training:** Train the model on the preprocessed dataset, emphasizing key features.
4. **Evaluation:** Assess the model's performance using metrics like Mean Squared Error and R².
   Files: Model.ipynb

## Resources Folder: 
This folder contains all of the csv files used to create our analysis, inlcuding the predicted 2023 values found in predicted_2023.csv. 

## Conclusion:

We rigorously evaluated our model's performance using metrics such as r squared. Our model had a high r squared value of 87%, allowing us to attain accurate predicted values. The feature which had the most significant impact on air quality was the 90th Percentage AQI value. After applying our model to the 2023 data, we attained a result of 3% for Mecklenburg and almost 1% for Raleigh. It is 3x the amount of unhealthy air pollutant days in Mecklenburg compared to Wake! We can also interpret these results as 97% Healthy and safe days Mecklenburg and Wake is predicted to have 99% healthy days for this year. Traffic, Transportation, and Population Density are all components which can influence air quality.

## Source: United States Environmental Protection Agency
https://aqs.epa.gov/aqsweb/airdata/download_files.html#Annual
