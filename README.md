# Weather Condition: A Python Project
![](https://github.com/FadilatBraimah/Weather-Condition-A-Python-Project/blob/c639014006b8a1e2553fe5502e24423dbf1ddfcc/weather_logo.jpg)

The Weather Dataset is a time-series data set with per-hour information about the weather conditions at a particular location. It records Temperature, Dew Point Temperature, Relative Humidity, Wind Speed, Visibility, Pressure, and Conditions. This document serves as a guide to the Jupiter Notebook used to analyze this  weather dataset.

## Weather Dataset Documentation
In this project, i utilizes two primary libraries for data manipulation and analysis:
- pandas: This library provides powerful data structures like DataFrames for handling tabular data.
- numpy: This library offers numerical computing capabilities used for some data analysis tasks.

## Dataset
The weather data was stored in a CSV file named "Project Weather Dataset.csv". I used the pandas.read_csv function to import this data into a pandas DataFrame named data_1. Containing 8784 entries and 8 columns, the dataset offers weather-related data for analysis and exploration. It contains a range of weather conditions, from clear skies to various forms of precipitation, including rain, snow, and drizzle, among others.

## Data Inspection
- Head: The head() method displays the first few rows of the DataFrame, providing a glimpse into the data's structure and content.
- Datatypes: The dtypes attribute reveals the data type associated with each column in the DataFrame. This helps understand how the data is represented (e.g., numerical values, text).
- Info: The info() method provides a summary of the DataFrame, including information about the number of rows and columns, data types, and memory usage.

## Data Analysis
In answering quesions about the weather condition of this dataset various functions were used in the code:
- Unique Wind Speeds: The code identifies all distinct values present in the "Wind Speed_km/h" column using the unique() method. It then calculates the total number of unique wind speeds using the nunique() method.
- Clear Weather Instances: The code determines the number of times the weather condition was "Clear" using two approaches:
- Filtering: I used this approach to select rows where the "Weather Condition" column matches "Clear". The value_counts() method then counts the occurrences.
- GroupBy: This approach groups the DataFrame by the "Weather Condition" column and retrieves the group corresponding to "Clear".
- Specific Wind Speed: The code brings rows where the "Wind Speed_km/h" column has a specific value (e.g., 4 km/h) using either boolean indexing or the get_group() method with groupby.
- Null Values: The isnull().sum() method is used to check for missing values (represented as NaN) in each column of the DataFrame.
- Column Renaming: The rename() method is used to modify the name of the "Weather" column to "Weather Condition" for better readability.
- Mean Visibility: The mean() method calculates the average visibility recorded in the dataset.
- Pressure Standard Deviation: The std() method computes the standard deviation of pressure values.
- Relative Humidity Variance: The var() method calculates the variance of relative humidity values.
- Containing Snow: The str.contains() method is used to identify rows where the "Weather Condition" column text includes "Snow" (e.g., "Snow Showers").
- High Wind & Good Visibility: In this code i select rows where the "Wind Speed_km/h" is greater than 24 and the "Visibility_km" is exactly 25

_*Check the ipynb file attached for proper analysis*_

![](https://github.com/FadilatBraimah/Weather-Condition-A-Python-Project/blob/c639014006b8a1e2553fe5502e24423dbf1ddfcc/thankyounote.jpeg)

_*Fadilat Braimah*_ 🥰
