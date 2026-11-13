# Data-Preparation-and-Analysis
This repository contains an end-to-end data preparation, exploratory data analysis (EDA), visualization, and feature engineering pipeline implemented in Python. 

1. Project Overview

This repository contains an end-to-end data preparation, exploratory data analysis (EDA), visualization, and feature engineering pipeline implemented in Python. Using transaction-level retail records from the Sample Superstore Dataset sourced from Kaggle, the project diagnoses profitability drivers, investigates discount elasticities, identifies regional performance disparities, and engineers machine-learning-ready features.


2. Dataset Information

Dataset Name: Sample Superstore Dataset (US Retail Analytics)
Source Platform: Kaggle (www.kaggle.com)
Format: Comma-Separated Values (Sample_Superstore.csv)
Dimensions: 1,000+ transaction rows, 20 initial attributes
Target Attributes: Sales, Profit, Discount, Quantity, Category, Sub-Category, Region, Segment, Order Date, Ship Date


3. Pipeline Architecture

Step 1: Dataset Collection & Setup
Specification of Kaggle source metadata, business problem statement, and six core analytical objectives.

Step 2: Python and NumPy Operations
High-performance array creation, multidimensional slicing, vectorized arithmetic, and statistical measures (mean, median, standard deviation, min, max, percentiles).

Step 3: Pandas Operations
DataFrame inspection, schema typing, first/last record extraction, summary metrics, null detection, and duplicate auditing.

Step 4: Data Cleaning & Preprocessing
Imputation of missing numerical and categorical features, duplicate pruning, datetime conversion, column standardization, and IQR outlier detection with a pre/post-cleaning audit table.

Step 5: Exploratory Data Analysis (EDA)
Univariate distribution shapes (skewness, kurtosis), categorical breakdowns, monthly aggregation trends, discount tier impact matrices, correlation analysis, and five data-driven observations.

Step 6: Data Visualization Using Matplotlib
Six publication-grade static figures: Log-scale Sales Histogram, Category Sales vs Profit Bar Chart, Monthly Trajectory Line Chart, Sales vs Profit Scatter Plot, Segment Box Plot, and Correlation Heatmap.

Step 7: Interactive Visualization Using Plotly
Three interactive figures: Marginal-box Sales Histogram, Multidimensional Sales-Profit Scatter Plot with detailed hover metadata, and Regional-Category Grouped Bar Chart, accompanied by business interpretations.

Step 8: Feature Engineering
Domain features (profit_margin, unit_price, shipping_duration_days, high_discount_flag), temporal feature extraction (year, month, quarter, day of week, weekend indicator), one-hot categorical encoding, and numerical scaling (StandardScaler and MinMaxScaler).

Step 9: Analysis and Conclusion
Synthesis of major operational findings, discount threshold patterns, three strategic business recommendations, and analytical dataset limitations.

Step 10: GitHub Submission Deliverables
Repository structure, execution steps, and environment specification.


4. Key Findings and Insights

Severe Margin Erosion Above 20% Discount: Orders with discounts exceeding 20% shift from an average positive profit to net operational losses.
Category Profitability Drivers: Technology products deliver the highest absolute margins, whereas Furniture suffers from volatile returns and heavy logistical discounting.
Regional Dynamics: The West and East geographic regions yield consistent profits, while the Central and South territories demonstrate vulnerabilities in furniture product categories.


5. Environment Setup and Execution

Local Setup
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
jupyter notebook data_preparation_and_analysis.ipynb
