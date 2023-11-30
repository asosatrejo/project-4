
# ☁️ Air Quality Analysis of North Carolina
This project will build a model to predict air quality in counties around North Carolina. We aim to predict with counties will have the most hazardous days, which will have the least, and whether there is an overall trend of air quilty improving or getting worse in the state.

# 🌤️ Why Choose Air Quality Analysis?
> Our group aims to create an algorithm that can predict air quality in different counties in North Carolina (NC). Air Quality can affect many people, including those with respiratory issues. As a group, we also feel passionate about protecting the enviroment and felt curious about the air quality of our own state. 

# 🌙 The Process

## Data Clean Up
### Obtain & Merge
The first step was to obtain and merge the csv files. After merging, `loc` was used to find all `North Carolina` rows. This was then saved as a new csv file titled `nc_aqi_2010-2022.csv`.

Data was inspected to understand its structure, missing values, and potential inconsistencies. Based on the inspection, ecessary cleaning steps were performed. Data was transformed as needed for analysis. Finally, data was then exported to `nc_aqi_2010-2022.csv`.

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

## Machine Learning

## Visualizations

## Analysis

# 🌞 Sources
We used CSV files from the United States Environmental Protection Agency as our source.
- [Pre-Generated Data Files](https://aqs.epa.gov/aqsweb/airdata/download_files.html#Annual)

> Project Created by Ariana, Mary, Natalie, and Jolyciel.
