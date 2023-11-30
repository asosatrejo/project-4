# ☁️ Environmental Data Analysis Project
## Overview:
This repository focuses on predicting healthy and unhealthy days' percentages in North Carolina by leveraging machine learning techniques. The project entails preprocessing and analyzing environmental data to gain insights into air quality trends. 

## Project Description:
The primary objective is to employ Linear Regression, facilitated by Scikit-learn, for predicting air quality metrics. The dataset, spanning from 1980 to 2023, includes comprehensive environmental information. Key tasks involve preprocessing and transforming the data to build a robust predictive model.

# 🌤️ Why Choose Air Quality Analysis?
> Our group aims to create an algorithm that can predict air quality in different counties in North Carolina (NC). Air Quality can affect many people, including those with respiratory issues. As a group, we also feel passionate about protecting the enviroment and felt curious about the air quality of our own state. 

# 🌙 The Process
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

# 2. Data Retrieval and Preprocessing

### 1. Loading the Data
- `pandas` is used to load the CSV file into a DataFrame.
- Initial data structure and contents are previewed with `data.head()`.

### 2. Data Inspection
- Checking for missing values with `data.isnull().sum()`.
- Ensuring data quality before proceeding with the analysis.

### 3. Data Cleaning
- Duplicate records are identified and removed using `data.drop_duplicates()`.
- The dataset’s integrity is maintained for accurate analysis.

### 4. Data Transformation
- Certain columns are converted to more efficient data types such as `category`.
- The changes are confirmed by re-checking the data types with `data.dtypes`.

### 5. Data Export
- The cleaned and processed DataFrame is exported to a new CSV file.
- This step provides a clean version of the dataset for future use.

### 6. Database Storage
- The dataset is stored in a SQLite database using `SQLAlchemy` for easy access and manipulation.
- Data is saved in table format, suitable for complex queries and analysis.

### 7. Feature Engineering
- New features are created based on existing data to provide more insights.
- Ratios and percentages are calculated to enrich the dataset.

## Linear Regression Model: 
1. **Target Variable Definition:** Clearly define the target variable - unhealthy days' percentages.
2. **Model Selection:** Choose Linear Regression for predicting air quality metrics.
3. **Training:** Train the model on the preprocessed dataset, emphasizing key features.
4. **Evaluation:** Assess the model's performance using metrics like Mean Squared Error and R².
   Files: Model.ipynb

# Resources: 
The folder labled as "Resources" contains all of the csv files used to create our analysis, inlcuding the predicted 2023 values found in predicted_2023.csv. 

# Conclusion:

We rigorously evaluated our model's performance using metrics such as r squared. Our model had a high r squared value of 87%, allowing us to attain accurate predicted values. The feature which had the most significant impact on air quality was the 90th Percentage AQI value. After applying our model to the 2023 data, we attained a result of 3% for Mecklenburg and almost 1% for Raleigh. It is 3x the amount of unhealthy air pollutant days in Mecklenburg compared to Wake! We can also interpret these results as 97% Healthy and safe days Mecklenburg and Wake is predicted to have 99% healthy days for this year. Traffic, Transportation, and Population Density are all components which can influence air quality.

# 🌞 Sources
We used CSV files from the United States Environmental Protection Agency as our source.
- [Pre-Generated Data Files](https://aqs.epa.gov/aqsweb/airdata/download_files.html#Annual)

> Project Created by Ariana, Mary, Natalie, and Jolyciel.
