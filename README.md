# Uber-Linear-Regression-Model
Orchestrated an astute data curation strategy, attending to outliers and conducting comprehensive data analysis. Imbued the analysis  with sophistication by employing label encoding and crafting a nuanced linear regression model.

1. **Data Import and Exploration**:
   - The code starts by importing necessary libraries like NumPy, Pandas, Matplotlib, Seaborn, and Datetime.
   - It reads the Uber trip data from a CSV file named "uber.csv" into a Pandas DataFrame named "df".
   - The `df.head()` function is used to display the first few rows of the dataset, allowing for initial data exploration.

2. **Data Preprocessing**:
   - The code drops the 'Unnamed: 0' and 'key' columns from the DataFrame, as they are considered irrelevant for the analysis. This is done using the `df.drop()` function with `axis=1` and `inplace=True` to make the changes permanent. 

3. **Data Information**:
   - The `df.info()` function is used to display information about the DataFrame, including the number of entries, column names, data types, and memory usage. 
   - The `df.shape` function is used to get the dimensions of the DataFrame, which is (200,000, 7), indicating 200,000 rows and 7 columns. 

4. **Missing Value Handling**:
   - The code checks for missing values in the DataFrame using the `df.isnull().sum()` function, which shows that there are 1 missing value each in the 'dropoff_longitude' and 'dropoff_latitude' columns. 

5. **Feature Engineering**:
   - The code adds new features to the DataFrame by extracting year, month, weekday, and hour from the 'pickup_datetime' column. This is done by converting the 'pickup_datetime' column to a datetime format. 

6. **Linear Regression Analysis**:
   - The code does not include the specific implementation of the linear regression model. However, the data preprocessing steps suggest that the next step would be to build and train a linear regression model using the Uber trip data to predict the 'fare_amount' based on the other features in the dataset.

In summary, the "Uber_Linear_Regression.ipynb" file focuses on preparing the Uber trip data for a linear regression analysis. It involves importing the data, dropping irrelevant columns, exploring the data, handling missing values, and performing feature engineering to extract additional information from the timestamp. The code sets the stage for applying a linear regression model to predict the fare amount based on the preprocessed features.
