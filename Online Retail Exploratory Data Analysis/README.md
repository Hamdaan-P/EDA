Project Overview

This repository contains an Exploratory Data Analysis (EDA) project on the Online Retail II dataset. The analysis explores transactional data from an online retail store spanning December 2009 to December 2011. It covers data cleaning, feature engineering, visualizations, and insights into sales trends, customer behavior, and product performance.
This project is part of my Data Science portfolio, showcasing skills in data manipulation, visualization, and deriving actionable insights using Python.
Objectives

Understand the structure and quality of the dataset.
Identify patterns, trends, and anomalies in sales data.
Analyze customer behavior and product performance.
Visualize key metrics for better interpretation.

Dataset

Source: UCI Machine Learning Repository (or similar; originally from online_retail_II.xlsx).
Description: Contains over 1 million transactions with columns like Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, and Country.
Sheets: "Year 2009-2010" and "Year 2010-2011" (combined in the analysis).
Size: Approximately 1,067,371 rows after loading.
Note: The notebook optimizes loading by converting Excel to CSV for faster performance on large files.

Tools and Technologies

Programming Language: Python
Libraries:

Pandas (data manipulation)
NumPy (numerical operations)
Matplotlib & Seaborn (data visualization)
Datetime (date handling)


Environment: Jupyter Notebook

Installation and Setup

Clone the repository:
git clone https://github.com/yourusername/online-retail-eda.git

Navigate to the project directory:
cd online-retail-eda

Install required dependencies:
pip install -r requirements.txt
Download the dataset (online_retail_II.xlsx) and place it in the project root. The notebook will handle conversion to CSV for efficiency.

Usage

Open the Jupyter Notebook:

jupyter notebook Online_Retail.ipynb

Run the cells sequentially. The notebook includes:

Data loading (with Excel to CSV optimization).
Cleaning (handling missing values, duplicates, data types).
Feature engineering (e.g., TotalPrice, date components).
Univariate, bivariate, and multivariate analyses.
Visualizations (histograms, bar plots, line plots, heatmaps, boxplots).
Customer analysis and outlier detection.



Key Findings and Insights

Data Quality: After cleaning, no missing critical values; focused on positive quantities and prices.
Sales Trends: Seasonal peaks, likely around holidays; monthly sales trends visualized.
Top Performers: UK dominates transactions and sales; popular products include decorative items like "WHITE HANGING HEART T-LIGHT HOLDER".
Customer Behavior: Small number of high-value customers drive revenue; peak sales during business hours.
Outliers: Identified in Quantity, Price, and TotalPrice via boxplots.
Recommendations: Focus on high-value customers, stock popular items, and consider international expansion.

Visualizations
Examples from the notebook:

Distribution of Quantity, Price, and TotalPrice (histograms).
Top countries and products (bar plots).
Monthly sales trends (line plot).
Correlation heatmap.
Sales by hour and weekday (heatmap).
Boxplots for outlier detection.

(For full visuals, run the notebook.)
Future Work

Implement RFM (Recency, Frequency, Monetary) analysis for customer segmentation.
Build predictive models (e.g., sales forecasting using time series).
Incorporate machine learning for anomaly detection or clustering.


Author

Name: Hamdaan Peshimam

GitHub: Hamdaan-P

LinkedIn: https://www.linkedin.com/in/hamdaan-peshimam-547394ba/

Email: phamdaan@gmail.com


Feel free to fork, star, or contribute! If you have questions or suggestions, open an issue.


