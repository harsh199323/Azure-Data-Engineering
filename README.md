# Azure-Data-Engineering
Tokyo Olympic Data Engineering 

# Tokyo Olympic Data Analysis with PySpark

This project uses PySpark to analyze and transform Tokyo Olympic data, including information about athletes, coaches, entries by gender, medals, and teams.

## Data Sources

The raw data is stored in Azure Data Lake Storage and is mounted to Databricks using Azure Blob File System (ABFS). The following datasets are used:

- `athletes.csv`
- `coaches.csv`
- `entriesgender.csv`
- `medals.csv`
- `teams.csv`

## PySpark Analysis

The PySpark code performs the following tasks:

1. **Data Loading**: Reads the raw CSV data into PySpark DataFrames for further analysis.

2. **Data Cleaning**: Ensures data types are appropriate and handles any necessary type conversions.

3. **Exploratory Data Analysis (EDA)**: Displays sample rows and prints the schema of each DataFrame.

4. **Top Gold Medal Countries**: Identifies and displays the top countries with the highest number of gold medals.

5. **Average Entries by Gender**: Calculates the average number of entries by gender for each discipline.

6. **Data Transformation**: Writes the transformed DataFrames to CSV files for future use.

## File Structure

- `raw-data/`: Contains the original raw CSV files.
- `transformed-data/`: Stores the transformed DataFrames after the PySpark analysis.

## How to Run

1. Set up the necessary configurations in the PySpark code, including Azure credentials.
2. Execute the code in a PySpark environment.

```python
# Example command to run the PySpark script
# (Replace with your actual script file name)
$ spark-submit your_script.py
