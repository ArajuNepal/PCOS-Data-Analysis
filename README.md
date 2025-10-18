# PCOS-Data-Analysis

This project consolidates multiple PCOS-related datasets into a single cleaned dataset for analysis and builds predictive models to identify PCOS based on health indicators. The main objectives are:

- Data Cleaning & Preprocessing: Merge datasets, handle missing values, and standardize data.
- Exploratory Data Analysis (EDA): Explore patterns and relationships between features and PCOS.
- Predictive Modeling: Build Logistic Regression and Random Forest models to predict PCOS.
- Data Export: Save cleaned and processed data for analysis and plotting.
  

# Key Features
1. Data Cleaning & Preprocessing
- Merges multiple datasets (Data_3.csv, Data_4.csv, Data_13.csv, PCOS_extended_dataset.csv) into a single unified dataset.
- Standardizes column names and formats.
- Converts categorical variables (e.g., Yes/No, blood group codes) to consistent formats.
- Handles missing values intelligently (probabilistic imputation for categorical variables, mean/BMI-based imputation for numeric variables).

2. Exploratory Data Analysis (EDA)
- Visualizes categorical and numerical variables using distribution plots, bar charts, and boxplots.
- Generates correlation heatmaps for numeric features.
- Performs Chi-square tests for categorical variables.
- Calculates point-biserial correlations between numeric variables and PCOS status.

3. Predictive Modeling
- Logistic Regression: Basic and refined models with exhaustive feature selection.
- Random Forest: Baseline and refined models with feature importance evaluation.
- Evaluation Metrics: Accuracy, Precision, Recall, F1 Score, ROC curve, and AUC.

4. Data Export
- Data_for_EDA.csv: Cleaned and merged dataset for analysis or modeling.
- boxplots_data.csv: Formatted dataset for plotting numeric variable distributions by PCOS status.


# Prerequisites 
- Python 3.8 or higher
- Recommended packages (install via requirements.txt)
  

# Installation
1. Clone the repository: git clone https://github.com/yourusername/PCOS-Data-Analysis.git
cd PCOS-Data-Analysis
2. Install dependencies: pip install -r requirements.txt
3. Place all raw CSV datasets into the data/ folder.


# Usage
1. Data Preprocessing & Merging
- Merge datasets, handle missing values, rename columns, and convert data types.

2. Exploratory Data Analysis (EDA)
- Visualize distributions, correlations, and associations between PCOS and features.
- Save plots using plt.savefig() if needed.

3. Predictive Modeling
- Train and evaluate Logistic Regression and Random Forest models.
- Use feature selection to improve model performance.
- Evaluate model using metrics like accuracy, precision, recall, F1 score, and AUC.

4. Export Processed Data
- Data_for_EDA.csv is ready for further analysis or modeling.
- boxplots_data.csv is ready for plotting numeric variable distributions by PCOS status.


# Notes
1. Missing categorical values are imputed based on probability distribution.
2. Numeric missing values for height and weight are filled using BMI-specific mean values.
3. Outliers and duplicates are removed; only individuals aged 15–45 are included.
4. Blood group and cycle regularity are encoded for modeling.
