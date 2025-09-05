# California Housing Data Analysis - Chapter 2

This project explores and prepares the California housing dataset for machine learning, following the steps in Chapter 2 of "Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow".

## Steps Completed

### 1. Data Loading
- Loaded the housing data from `housing.csv` using pandas.

### 2. Data Exploration
- Displayed the first few rows with `df.head()`.
- Used `df.info()` to inspect data types and missing values.
- Checked value counts for the categorical feature `ocean_proximity`.
- Used `df.describe()` to view summary statistics for numerical features.

### 3. Data Visualization
- Plotted boxplots for numerical features to visualize quartiles and outliers.
- Plotted histograms to examine the distribution of each numerical attribute.
- Created scatter plots to visualize geographic data (`longitude` vs `latitude`) and relationships between features (e.g., `median_income` vs `median_house_value`).
- Used scatter matrix plots to visualize pairwise relationships between selected features.

### 4. Feature Engineering for Stratified Sampling
- Created an `income_cat` feature by binning `median_income` into categories for stratified sampling.
- Visualized the distribution of `income_cat`.

### 5. Train-Test Splitting
- Performed a random train-test split using `train_test_split` (for comparison).
- Performed a **stratified train-test split** using `StratifiedShuffleSplit` to ensure the train and test sets have similar proportions of income categories.

### 6. Data Cleaning
- Removed the `income_cat` column from the train and test sets after splitting.

### 7. Correlation Analysis
- Computed the correlation matrix for numerical features to identify relationships with the target variable (`median_house_value`).

---

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

## Next Steps

- Further feature engineering
- Handling missing values
- Preparing data for machine learning models

---

*This notebook provides a solid foundation for building and evaluating machine learning models on California