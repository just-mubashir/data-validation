Code Overview

This code is a Python script that performs data analysis and visualization on a dataset using 
PySpark and various data analysis libraries. The purpose of this script is to load and analyze the data,
perform basic data cleaning, generate various types of visualizations, 
and run checks for data integrity and anomalies.

Requirements

To run this script, you need to have the following libraries installed:

PySpark
pandas
numpy
matplotlib
seaborn
pydeequ

You can install the required libraries using the following command:

pip install pyspark pandas numpy matplotlib seaborn pydeequ

How to Use

Import required libraries and set up the Spark session:

Set the Spark version to 3.1.
Import necessary libraries, including PySpark, pandas, numpy, matplotlib, seaborn, and pydeequ.
Create a Spark session named "testData".


Load data from a CSV file named "testData.csv" into a Spark DataFrame called data.
Convert the Spark DataFrame to a pandas DataFrame named df.

Data Cleaning and Preprocessing:

Perform initial data cleaning by dropping rows with missing values.
Round numerical columns to 3 decimal places and cast them to integers.

Basic Data Analysis and Visualization:

Display basic information about the data, including the schema and the first few rows.
Define a function my_count to display the count of non-null values in each column.
Display counts for each column using the my_count function.
Generate summary statistics and a histogram for selected columns.
Group data by "price" and display counts for each price value.
Define a function histogram to create a histogram for a given column.
Define a function lineplot to create line plots based on different aggregation measures.
Create line plots for "price" vs. "bed" and "acre_lot" vs. "price".
Group data by "status" and count occurrences of each status value.
Define a function pieplot to create a pie chart for a given column.
Create a pie chart for "price" with a specific status value.
Data Transformation and Column Manipulation:

Clean column names by removing whitespaces and dots.
Modify the "status" column by calculating a new value based on existing columns.
Filter data based on specific conditions using the filter function.
Modify the "status" column based on conditional expressions.
Data Quality Checks and Profiling.

These sections involve checks for data integrity, completeness, uniqueness, and more.
Profiling and anomaly detection.

Running the Script

To run the script, make sure you have Python and the required libraries installed. You can execute the script in a Jupyter Notebook or any Python environment that supports the libraries used in the code.

Please note that some parts of the code are commented out (indicated by #) and are meant for additional data quality checks and profiling. Uncomment these sections if you want to perform those analyses.

Remember to update the data file name and adjust paths if necessary.
