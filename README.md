# financial-crisis-visualization
Exploratory Data Analysis on 2008 World Financial crisis and run dynamics

The notebook does simple data visualizations on historical financial data for distressed institutions (AIG, Citigroup, JPMorgan) and market stress indicators (VIX volatility index, TED Rate, S&P 500, Dow Jones) during the crises. 

# financial-crisis-visualization

### 📉 Exploratory Data Analysis on the 2008 Global Financial Crisis

This repository contains a Jupyter Notebook that performs an exploratory data analysis (EDA) on the 2008 financial crisis. It focuses on programmatically ingesting, cleaning, and visualizing historical tick data to identify the mechanical breakdowns in market confidence.

The analysis specifically correlates the collapse of distressed institutions (like **AIG**) against broader system stress indicators.

### 🚀 Key Features

* **Automated Data Pipeline**: Scripts to unzip and inventory complex financial datasets (`gfc.zip`) containing equities and macro indicators.
* **Data Cleaning**: Routines to parse raw CSVs, handle missing values, and convert string-based pricing data into numeric formats for analysis.
* **Visualization**: Time-series plotting using `Matplotlib` to track the volatility and collapse of key financial players.
    * *Primary Focus*: **American International Group (AIG)** stock price trajectory (Open/High/Low/Close) during the crisis window.
* **Macro Context**: Setup for analyzing systemic risk factors, including the **TED Rate**, **VIX Volatility Index**, and **Treasury Yields** (`WGS3MO`).

### 🛠️ Technologies Used

* **Python 3.x**
* **Pandas**: For data manipulation and time-series indexing.
* **Matplotlib**: For generating financial charts.
* **Zipfile**: For handling compressed data archives programmatically.

### 📂 Repository Structure

```text
├── Databusters_ Financial Crises 2008 analysis.ipynb   # Main analysis notebook
└── README.md                                           # Project documentation
