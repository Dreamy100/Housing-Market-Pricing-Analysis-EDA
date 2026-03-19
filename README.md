# Housing Market Pricing Analysis

## Overview

This project analyzes housing sales data from King County to understand the key factors that influence property prices. The focus is on identifying patterns in pricing, evaluating the impact of property features, and uncovering relationships that can inform real-world real estate decisions.

The analysis is conducted using Python in a notebook-based workflow, combining data exploration, visualization, and interpretation to extract meaningful insights from the dataset.

---

## Project Objectives

* Understand the distribution of housing prices
* Identify the key drivers of property value
* Analyze how features like size, location, and condition affect pricing
* Detect patterns and anomalies in the housing market
* Build a structured analytical workflow for real-world data problems

---

## Project Structure

```text
HOUSING MARKET PRICING ANALYSIS/
│
├── data/
│   └── kc_house_data.csv     # Dataset
|
│── tableau/
│   ├── tableau_dashboard.twbx
│   ├── visualization_full.pdf    # Tableau Visualizations
│   └── dashboard_preview.png
|
├── housing_venv/             # Virtual environment (not tracked)
├── housing_analysis.ipynb    # Main analysis notebook
├── .gitignore                # Ignored files
├── requirements.txt          # Dependencies
├── README.md                 # Project documentation
├── LICENSE                   # License
```

---

## Dataset

The dataset contains housing sales data with features such as:

* Price
* Number of bedrooms and bathrooms
* Square footage (living space, lot size)
* Floors and property condition
* Waterfront and view indicators
* Location-related attributes
* Year built and renovation details

---

## Approach

### 1. Data Exploration

* Examined dataset structure and summary statistics
* Identified missing values and inconsistencies
* Explored distributions of key variables

### 2. Data Cleaning

* Handled missing or inconsistent values
* Ensured correct data types for analysis
* Removed or evaluated outliers where necessary

### 3. Feature Analysis

* Studied relationships between price and:

  * Living area (sqft)
  * Number of bedrooms and bathrooms
  * Property condition and grade
  * Location and special features (e.g., waterfront, view)

### 4. Visualization

* Distribution plots to understand price spread
* Scatter plots to analyze relationships between variables
* Comparative plots for categorical features

---

## Exploratory Data Analysis

### 1. Price Distribution
- Right-skewed distribution with luxury outliers inflating average prices  

---

### 2. Key Price Drivers

- **Living Area (sqft_living):** Strongest driver; larger homes command higher prices  
- **Bedrooms:** Price increases initially, then shows diminishing returns  
- **Bathrooms:** Stronger impact than bedrooms, reflecting comfort/luxury value  

---

### 3. Property Quality

- **Grade:** Major price driver; higher construction quality significantly increases value  
- **Condition:** Impacts price but less than grade  

---

### 4. Premium Features

- **Waterfront:** Significant price premium  
- **View:** Higher ratings correlate with higher prices  

---

### 5. Geographic Analysis

- **Zipcodes:** High-value properties concentrated in specific regions  
- **Spatial Patterns:** Clear clustering of expensive homes (lat-long analysis)  

---

### 6. Price per Square Foot
- Key benchmarking metric; varies significantly across locations  

---

### 7. Property Age
- Newer homes priced higher; older homes show greater variability  

---

### 8. Market Segmentation
- Segmented into Low / Mid / High tiers to analyze distribution  

---

### 9. Cross Analysis (Bedrooms × Grade)
- Bedroom impact depends on grade; high-grade homes outperform across levels  

---

### 10. Market Trends
- Moderate seasonal variation in monthly pricing  
---

## Key Insights

* **Living area (sqft) is one of the strongest predictors of price**
  Larger homes consistently command higher prices, though with diminishing returns at extreme values.

* **Property grade and condition significantly impact pricing**
  Higher-grade homes show a clear upward shift in price distribution.

* **Waterfront and view properties carry a substantial premium**
  These features create distinct clusters of higher-priced homes.

* **Bedrooms alone are not a strong predictor of price**
  Properties with similar bedroom counts can vary widely in price depending on size and quality.

* **Outliers exist in both directions**
  Some properties are priced significantly higher or lower than expected, indicating unique characteristics or potential data irregularities.

---

## Visualization Highlights

The project includes:

- Price distribution histogram
- Scatter plots (price vs sqft, bathrooms, age)
- Boxplots (bedrooms, grade, condition, waterfront)
- Geographic scatter plot (lat vs long with price)
- Zipcode-wise bar charts
- Correlation heatmap
- Monthly trend line chart

---

## Tools and Technologies

* Python
* Jupyter Notebook
* Pandas
* Numpy
* Matplotlib / Seaborn

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/housing-market-pricing-analysis.git
cd housing-market-pricing-analysis
```

2. Create and activate virtual environment:

```bash
python -m venv housing_venv
source housing_venv/bin/activate   # Mac/Linux
housing_venv\Scripts\activate      # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the notebook:

```bash
jupyter notebook housing_analysis.ipynb
```

---

## Key Takeaways

* Housing prices are driven by a combination of **size, quality, and premium features**, rather than any single variable.
* Simple metrics (like bedroom count) are often misleading without context.
* Visualization is essential for uncovering patterns that are not obvious from raw data.
* A structured approach to data analysis leads to clearer and more reliable insights.

---

## Notes

This project focuses on understanding the data from an analytical perspective rather than building a predictive model. The emphasis is on clarity, interpretation, and developing intuition around how different variables influence housing prices.

---

## Acknowledgements

Dataset sourced from publicly available real estate transaction data.

---

## License

This project is licensed under the terms of the LICENSE file included in this repository.

