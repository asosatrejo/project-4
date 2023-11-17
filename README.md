# Air Quality Analysis
## In North Carolina

# Why Choose Air Quality Analysis?
> Our group aims to create an algorithm that can predict air quality in different counties in North Carolina (NC). Air Quality can affect many people, including those with respiratory issues. As a group, we also feel passionate about protecting the enviroment and felt curious about the air quality of our own state. 

# The Process

## Data Clean Up
### Obtain & Merge
The first step was to obtain and merge the csv files. After merging, `loc` was used to find all `North Carolina` rows. This was then saved as a new csv file titled `nc_aqi_2010-2022.csv`.
### Data Inspection, Cleaning, and Transformation
Data was inspected to understand its structure, missing values, and potential inconsistencies. Based on the inspection, ecessary cleaning steps were performed. Data was transformed as needed for analysis. Finally, data was then exported to `nc_aqi_2010-2022.csv`.
### Database Storage
SQLALCHEMY was used to create an engine that will store the data in a table named `air_quality_data`.

## Machine Learning

## Visualizations

## Analysis

# Sources
We used CSV files from the United States Environmental Protection Agency as our source.
- [Pre-Generated Data Files](https://aqs.epa.gov/aqsweb/airdata/download_files.html#Annual)

> Project Created by Ariana, Mary, Natalie, and Jolyciel.