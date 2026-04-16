Aim
To perform preprocessing on a dataset and handle missing values using Python (Pandas & NumPy).

Theory
Data preprocessing is a critical step in any data analysis or machine learning pipeline. Real-world datasets are often incomplete, inconsistent, or incorrectly formatted. Preprocessing ensures the data is clean, structured, and ready for analysis.
Key concepts covered:

Missing Values: Represented as NaN (Not a Number) in Pandas. These arise due to data entry errors, sensor failures, or incomplete records.
Detection: isna() returns a boolean mask of missing entries; notna() returns the inverse. isna().sum() gives a count of missing values column-wise or row-wise.
Dropping Missing Data: dropna() removes rows (or columns) that contain any NaN values.
Filling Missing Data: fillna() replaces NaN with a specified value, the column mean, median, or any custom strategy.
Type Conversion: pd.to_numeric() with errors='coerce' converts invalid entries to NaN safely.
Standardisation: Inconsistent text (e.g., "cse" vs "CSE") is normalised using .str.upper() or .str.lower().
Date Parsing: pd.to_datetime() with format='mixed' handles multiple date formats in the same column.


Conclusion
The experiment successfully demonstrated how to identify and handle missing values in a Pandas DataFrame. Techniques such as isna(), dropna(), and fillna() were used on a simple DataFrame, followed by a more realistic dataset containing mixed data types, inconsistent formatting, and irregular date formats. Missing numeric values were imputed using mean and median, text columns were standardised to uppercase, and date columns were parsed into a uniform datetime format. These preprocessing steps are essential for producing reliable and accurate analytical results.

Libraries Used
LibraryPurposepandasDataFrame operations, missing value handling, type conversionnumpyGenerating NaN values
