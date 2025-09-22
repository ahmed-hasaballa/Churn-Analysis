# Churn-Analysis: -

Purpose
This notebook performs exploratory data analysis (EDA), preprocessing, modelling and evaluation for a customer churn dataset.

Quick facts: -
Notebook file: churn analysis.ipynb (uploaded).
Number of cells: 45 (automatically detected).
Detected Python libraries (sample): pandas, numpy, matplotlib.pyplot, seaborn, sklearn.preprocessing.
Detected dataset path (from read_csv):

Requirements: -
Python 3.8+ recommended (should work with 3.7+).
Core packages used (install with pip):

!pip install pandas numpy matplotlib seaborn scikit-learn joblib

Setup / Imports: -
Installs/imports commonly used libraries (pandas, numpy, matplotlib, seaborn, sklearn.*).
What to check: that imports succeed and the environment has compatible package versions.

Data Loading: -
The notebook reads the CSV into a DataFrame using pd.read_csv(...) (path detected above).
What to check: file path, delimiter, encoding. If you get FileNotFoundError, update the path or move the CSV next to the notebook.

Initial inspection: -
df.head(), df.shape, df.dtypes, df.describe() and df.info() to inspect columns, types and sample rows.
What to look for: target column (e.g., Churn), numeric vs categorical columns, unexpectedly high missingness.

Missing values & duplicates check: -
Calls like df.isna().sum() and duplicate checks appear in the notebook.
Typical actions: drop duplicates, impute or drop missing values.

Exploratory Data Analysis (EDA): -
Distribution plots, countplots and correlation/heatmap across features.
What to check: class imbalance for the churn target, strongly correlated features, outliers.

Preprocessing: -
Categorical encoding (e.g. pd.get_dummies, LabelEncoder) and numeric scaling (e.g. StandardScaler, MinMaxScaler) may be used.
Missing value imputation with fillna or SimpleImputer may be present.
What to check: ensure target column is excluded from scaling/encoding when appropriate; confirm encoding method for high-cardinality categorical variables.
