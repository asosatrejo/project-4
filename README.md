# project-4

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
