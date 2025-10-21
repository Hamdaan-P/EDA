# 🛒 Amazon Sales Report Exploratory Data Analysis (EDA)

## Project Overview

This project is an Exploratory Data Analysis (EDA) of the Amazon Sales Report dataset. The primary goal is to derive actionable business insights from transactional data, focusing on sales trends, product performance, fulfillment efficiency, and customer segmentation (B2B vs. Individual).

The analysis is performed using Python in a Jupyter Notebook environment, utilizing popular data science libraries for cleaning, transformation, and visualization.

## 💾 Dataset

The analysis is based on the **Amazon Sale Report** dataset, commonly found on platforms like Kaggle. The notebook assumes the CSV file, named `Amazon Sale Report.csv`, is located in the same directory as the Jupyter Notebook.

### Key Columns Analyzed:
* **Date**: For tracking monthly and seasonal trends.
* **Category**: To identify top-selling product categories.
* **Amount**: The revenue generated for each transaction.
* **Fulfilment**: To compare Amazon-fulfilled vs. Merchant-fulfilled orders.
* **B2B / Customer Type**: To distinguish between business and individual customers.

## 📊 Analysis Highlights

The EDA covers the following key areas:

1.  **Data Cleaning & Preprocessing**: Handling missing values, dropping irrelevant columns (`index`, `Unnamed: 22`, etc.), and converting data types (`Date` to datetime).
2.  **Time-Series Analysis**: Visualizing **Monthly Sales Trend** to identify performance over time.
3.  **Product Performance**: Bar chart visualization of **Top 10 Product Categories by Total Sales**.
4.  **Logistics Analysis**: Pie chart showing the distribution of sales by **Fulfillment Method** (Amazon vs. Merchant).
5.  **Customer Segmentation**: Analyzing **Order Volume and Sales Value** split between B2B (Business) and Individual customers.
6.  **Multivariate Analysis**: Stacked bar chart examining the **Top Category Sales by Fulfillment Method** to inform inventory strategy.

## 🚀 How to Run the Project

### Prerequisites

You need Python installed on your system. It's highly recommended to use a virtual environment.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Hamdaan-P/EDA.git
    cd EDA
    ```

2.  **Create and activate a virtual environment (optional but recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Linux/macOS
    venv\Scripts\activate      # On Windows
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Obtain the Dataset:**
    * Download the `Amazon Sale Report.csv` file from the source (e.g., Kaggle).
    * Place the CSV file in the root directory of this project.

5.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```

6.  Open the `Amazon_Sales_Report_EDA.ipynb` file and run all cells sequentially to reproduce the analysis.

## 🤝 Contributing

Feel free to open issues or submit pull requests for improvements, additional analyses, or alternative visualizations.


---
