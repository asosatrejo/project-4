# ☁️ Environmental Data Analysis Project
## Overview:
This repository focuses on predicting healthy and unhealthy days' percentages in North Carolina by leveraging machine learning techniques. The project entails preprocessing and analyzing environmental data to gain insights into air quality trends. 

## Project Description:
The primary objective is to employ Linear Regression, facilitated by Scikit-learn, for predicting air quality metrics. The dataset, spanning from 1980 to 2023, includes comprehensive environmental information. Key tasks involve preprocessing and transforming the data to build a robust predictive model.

# 🌤️ Why Choose Air Quality Analysis?
> Our group aims to create an algorithm that can predict air quality in different counties in North Carolina (NC). Air Quality can affect many people, including those with respiratory issues. As a group, we also feel passionate about protecting the enviroment and felt curious about the air quality of our own state. 

# 🌙 The Process
## Pre-Processing Steps:
1. **Data Cleaning:** Address missing values and handle outliers to ensure data integrity. Focusing on North Carolina counties.
   ![image](https://github.com/asosatrejo/project-4/assets/135572871/b9e239d9-845b-4300-8716-9cdc6f62d7b2)
3. **Data Transformation:**  Certain columns are converted to more efficient data types.
4. **Feature Engineering:** Derive meaningful features such as the Unhealthy Days percentage from raw data.
5. **2023 Data:** Finding Data for Mecklenburg and Wake county in order to fit into our model
   ![image](https://github.com/asosatrejo/project-4/assets/135572871/84f0113a-2ea7-4fa1-8b20-3795f8eea7fb)
### Files
`meck_co.ipynb`, `merge-csv.ipynb`, `nc_2023_data.ipynb`, and `updated_analysis_notebook.ipynb`

## Data Storage in SQL:
1. **Database Storage:** Data is saved in table format, suitable for complex queries and analysis.
2. **Data Migration:** Transfer the preprocessed data into the SQL database for efficient storage and retrieval.
   ![image](https://github.com/asosatrejo/project-4/assets/135572871/4a5aa336-2cf1-4c6b-ab58-eb618a4bbd3a)

### Files
`nc_aqi_data.db` and `updated_database.ipynb` 

## Linear Regression Model: 
1. **Target Variable Definition:** Clearly define the target variable - unhealthy days' percentages.
2. **Model Selection:** Choose Linear Regression for predicting air quality metrics.
3. **Training:** Train the model on the preprocessed dataset, emphasizing key features.
4. **Evaluation:** Assess the model's performance using metrics like Mean Squared Error and R².
   ![image](https://github.com/asosatrejo/project-4/assets/135572871/a8447227-2553-49a5-bf0f-0e1fd911f344)

### Files
`Model.ipynb`

## Tableau Dashboard:
1. **Past Patterns and Future Predictions:** Showcases predicted pollutant concentrations for 2023 based on previous data
2. **Exploring Relationships in Exposure Levels:** Highlights pollutant pairings in Mecklenburg and Wake County
3. **90th Percentile Analysis:** Demonstrates line graph of air quality over time.

**View [Tableau](https://public.tableau.com/app/profile/mary.feaster/viz/EnvironmentalMLAnalyticsNCUrbanAreas/Story1) Dashboard**

# 📁 Resources: 
- Presentation Slides: `Environmental ML Analytics.pdf`

Resources Folder contains:
- 📂 Annual_AQI_1980-2022
  - Contains CSV files later merged into `c_aqi_1980-2022.csv`.
  - Merged CSV file was used to train data.
- 📂 Pollutant_Data
  - Contains CSV files later merged into `nc_2023_data.csv`.
  - - This is data used to input into the model.
- `cleaned_data.csv`
- `predicted_2023.csv` - Output from model.

# ☁️ Conclusion:
We rigorously evaluated our model's performance using metrics such as r squared. Our model had a high r squared value of 87%, allowing us to attain accurate predicted values. The feature which had the most significant impact on air quality was the 90th Percentage AQI value. After applying our model to the 2023 data, we attained a result of 3% for Mecklenburg and almost 1% for Raleigh. It is 3x the amount of unhealthy air pollutant days in Mecklenburg compared to Wake! We can also interpret these results as 97% Healthy and safe days Mecklenburg and Wake is predicted to have 99% healthy days for this year. Traffic, Transportation, and Population Density are all components which can influence air quality.

Overall, when displaying our data, the air quality is getting better!

# 🌞 Sources
- [Pre-Generated Data Files](https://aqs.epa.gov/aqsweb/airdata/download_files.html#Annual)
- [Download Daily Data](https://www.epa.gov/outdoor-air-quality-data/download-daily-data)
- [Air Data Basic Information](https://www.epa.gov/outdoor-air-quality-data/air-data-basic-information#:~:text=The%20AQI%20is%20an%20index,runs%20from%200%20to%20500.)
- [About Air Data Reports](https://www.epa.gov/outdoor-air-quality-data/about-air-data-reports)

> Project Created by Ariana, Mary, Natalie, and Jolyciel.
