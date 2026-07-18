# databricks-flight-data-analysis
Flight data analysis and machine learning project using PySpark and Databricks, covering data cleaning, transformations, feature engineering, and ML pipelines.
# Flight Data Analysis and Machine Learning with PySpark

## Project Overview

This project demonstrates data processing, analysis, and machine learning using PySpark in Databricks. The project uses flight and airport datasets to explore flight information, clean and transform the data, perform aggregations, and prepare features for machine learning.

## Technologies Used

- Databricks
- Apache Spark
- PySpark
- Spark SQL
- PySpark MLlib
- Python

## Project Workflow

### 1. Data Ingestion
- Loaded flight and airport CSV datasets into Databricks.
- Read the datasets using PySpark DataFrames.
- Explored the dataset schema and column information.

### 2. Data Cleaning and Transformation
- Handled invalid values such as `NA`.
- Converted columns to appropriate numeric data types using `try_cast`.
- Created new calculated columns.
- Selected and filtered data using the PySpark DataFrame API.

### 3. Data Analysis
Performed different operations including:

- Filtering flight records.
- Grouping data by origin and destination.
- Calculating minimum and average values.
- Generating summary statistics.
- Calculating average flight speed.

### 4. Data Integration
- Joined flight data with airport information.
- Used airport codes to connect flight destinations with airport details.

### 5. Feature Engineering
Prepared categorical and numerical features for machine learning using:

- `StringIndexer`
- `OneHotEncoder`
- `VectorAssembler`

Categorical columns such as carrier and destination were converted into numerical representations suitable for machine learning models.

### 6. Machine Learning Pipeline
Created a PySpark ML Pipeline to automate the feature engineering process.

The pipeline includes:

1. String indexing
2. One-hot encoding
3. Feature vector assembly

The processed dataset was then split into training and testing datasets.

### 7. Model Training and Evaluation
- Trained machine learning models using the prepared feature data.
- Used cross-validation for model tuning and model selection.
- Evaluated model performance on test data.

## Key Learnings

Through this project, I gained hands-on experience with:

- PySpark DataFrame operations
- Spark SQL expressions
- Data cleaning and type conversion
- Data aggregation and joins
- Handling categorical features
- Building PySpark ML pipelines
- Training and validating machine learning models
- Working with Databricks and Unity Catalog Volumes

## Repository Structure

flight-data-pyspark/
├── notebooks/
│   └── flight_data_analysis.ipynb
└── README.md

## Future Improvements

- Add more exploratory data analysis and visualizations.
- Experiment with additional machine learning models.
- Compare model performance using different evaluation metrics.
- Build a complete data engineering pipeline using the Medallion Architecture.
