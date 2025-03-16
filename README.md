The AB_NYC_2019 dataset contains Airbnb listings in New York City, including details about pricing, location, host information, and reviews. Cleaning this dataset is essential for accurate analysis and machine learning models.

Key Data Cleaning Steps:
Handling Missing Values:

Identify missing values using .isnull().sum()
Fill missing values with appropriate techniques:
Mean/median for numerical columns (e.g., reviews_per_month)
Mode or "Unknown" for categorical columns (e.g., host_name)
Drop columns with excessive missing data if needed
Handling Duplicates:

Remove duplicate rows using .drop_duplicates()
Fixing Data Types:

Convert last_review to datetime format (pd.to_datetime())
Ensure numerical columns are correctly formatted
Outlier Detection & Removal:

Detect extreme values in price using boxplots
Remove unrealistic prices (e.g., listings with price = 0 or extremely high values)
Standardizing Text Data:

Convert text to lowercase for consistency
Remove unnecessary white spaces
Encoding Categorical Variables (if needed for ML):

Convert categorical variables (neighbourhood_group, room_type) into numerical format using one-hot encoding or label encoding

Conclusion
Cleaning the AB_NYC_2019 dataset ensures higher data quality, leading to more accurate analysis and predictions.
