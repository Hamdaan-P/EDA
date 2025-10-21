# New York City Airbnb Exploratory Data Analysis (EDA)

## 📊 Project Overview

This project presents a comprehensive Exploratory Data Analysis (EDA) of the 2019 New York City Airbnb dataset. The goal was to uncover key trends, price drivers, and geographical distribution patterns of short-term rentals in the five boroughs.

The analysis demonstrates proficiency in **data cleaning, missing value imputation, robust outlier handling, and creating high-impact visualizations** to derive actionable business insights.

## ⚙️ Methodology & Techniques

The analysis was executed in an iterative process to ensure data quality and maximize insight generation:

1.  **Data Loading & Initial Assessment:** Used `pandas` to load the `AB_NYC_2019.csv` file and conducted preliminary checks using `.info()`, `.describe()`, and `.isnull().sum()`.
2.  **Robust Data Cleaning & Preprocessing:**
    * **Missing Value Imputation:** Imputed missing values in `reviews_per_month` with `0`, based on the logical assumption that a missing value indicates no reviews.
    * **Feature Engineering/Selection:** Dropped high-cardinality/low-value columns (`id`, `host_name`, `last_review`) to streamline the analysis.
3.  **Advanced Outlier Handling (Price):** Implemented a multi-step outlier removal strategy for the crucial `price` column:
    * Removed listings with price = 0 (unrealistic data entry).
    * Applied the **Interquartile Range (IQR) method** to identify and cap extreme high-end prices (e.g., listings > $1000), ensuring a clean and representative distribution for statistical modeling.
4.  **Exploratory Data Analysis (EDA):** Performed univariate, bivariate, and multivariate analysis using `matplotlib` and `seaborn`.

## ✨ Key Findings & Insights

### 1. Geographical Price Disparity
* **Manhattan** consistently holds the highest median price across all neighbourhood groups, followed by Brooklyn. This confirms its status as the most expensive borough for short-term rentals.
* **Geospatial Analysis** revealed dense clusters of high-priced listings concentrated in specific, high-demand Manhattan neighbourhoods like Midtown and Chelsea.

### 2. Room Type is the Primary Price Driver
* The **`Entire home/apt`** room type has a significantly higher median price and price variance compared to `Private room` and `Shared room`, establishing it as the most influential factor on listing price.

### 3. Review Volume vs. Location
* Listings in **Brooklyn** and **Manhattan** show the highest average number of reviews, suggesting greater rental volume and popularity in these major tourist/business hubs.

### 4. Correlation Analysis
* A weak, slightly **negative correlation** was observed between `price` and `number_of_reviews`, suggesting that older, high-volume, well-reviewed listings may tend to be priced more affordably than new, boutique, or highly premium listings.

## 📦 Project Files

* `New_York_City_Airbnb_EDA.ipynb`: The primary Jupyter Notebook containing all the Python code for data loading, cleaning, analysis, and visualization.
* `AB_NYC_2019.csv`: The raw dataset used for this project.
* `README.md`: Project description and overview.
* `requirements.txt`: List of required Python libraries.

## 🛠️ Prerequisites

To run this project locally, you will need **Python 3.7+** installed. The following libraries are required and can be installed via the `requirements.txt` file.

## 🚀 Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Hamdaan-P/EDA.git
    cd EDA
    ```
2.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the analysis:**
    Open the Jupyter Notebook and execute the cells:
    ```bash
    jupyter notebook New_York_City_Airbnb_EDA.ipynb

    ```
