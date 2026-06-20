# Car Sales Data Analysis Project 🚗📊

Welcome to the **Car Sales Analysis** repository! This project demonstrates hands-on proficiency in data ingestion, data cleaning, complex querying, and insightful data visualization using Python's **Pandas** library within **Google Colab**.

The primary objective of this project is to analyze a comprehensive car sales dataset (`car_prices.csv`) to uncover market trends, pricing patterns, vehicle condition impacts, and regional sales performance.

---

## 🛠️ Tech Stack & Environment
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Google Colab / Jupyter Notebook

---

## 🚀 Key Features & Project Workflow

### 1. Data Ingestion & Quality Profiling
Before diving into analysis, a thorough data audit and cleaning pipeline were established:
* **Load & Inspect:** Imported `car_prices.csv` into a Pandas DataFrame and inspected structural metadata (shape, column data types, record counts, and the first 5 records).
* **Missing & Anomaly Detection:** * Quantified null values per column and visualized the missingness using heatmaps/bar charts.
    * Handled missing values systematically based on data type and the missingness percentage.
    * Identified, quantified, and removed duplicate records to ensure data integrity.

### 2. Dataframe Queries & Business Logic
Leveraged Pandas methods (grouping, filtering, aggregations, and window functions) to solve 12 critical business questions:
* **Aggregations:** Calculated baseline stats (average, min, max) for car prices.
* **Cardinality Checks:** Identified unique car colors, brands (makes), and specific models.
* **Premium Segment Analysis:** Filtered high-value inventory (selling prices > $165,000).
* **Market Demand:** Isolated the top 5 most frequently sold car models.
* **Grouped Insights:** Analyzed average selling price by brand, and minimum price by interior type.
* **Feature Engineering:** * Created a dynamic `car_age` column (calculated using the baseline year of 2025).
    * Sorted and ranked historical high-odometer readings by year.
* **Advanced Filtering:** Targeted high-wear/high-performance vehicles (Condition $\ge$ 48 & Odometer > 90,000 miles).
* **Geospatial & Value Analysis:**
    * Identified which US states consistently yield higher prices for newer cars (Year > 2013).
    * Discovered "Value for Money" brands by analyzing the lowest average prices within the top 20% excellent-condition tier.

### 3. Data Visualization & Insights
Data was translated into actionable business intelligence using Matplotlib and Seaborn:
* **Feature Correlation:** A heatmap showing the mathematical relationship among numerical features (Price, Odometer, Condition).
* **Temporal Trends:** Line/Bar charts tracking the average selling price over years to dissect market inflation or depreciation trends.
* **Odometer vs. Price:** Scatter plots visualizing the impact of mileage on market valuation.
* **Geographic Density:** A distribution chart mapping vehicle sales volume by state to pinpoint the top 3 highest-selling regions.
* **Condition Scoring Analytics:** * Bar charts binning condition scores into ranges of 5 to measure pricing elasticity.
    * Volume distribution charts binning condition scores into ranges of 10.
* **Outlier & Distribution Analysis:** Box plots highlighting price distributions grouped by car color, including a dedicated pass to identify and remove statistical outliers for cleaner insights.

---

## 📂 Repository Structure
```text
├── Data/
│   └── car_prices.csv          # Source dataset (or link to dataset if large)
├── Notebooks/
│   └── Car_Sales_Analysis.ipynb # Google Colab/Jupyter Notebook with full source code
└── README.md                   # Project documentation# Used-Car-Sales-Analysis
The objective of this Project is to develop hands-on proficiency in data analysis using the Pandas library in Python, i extract meaningful business insights, visualize key trends, and apply foundational techniques for exploratory data analysis (EDA) in a practical context.
