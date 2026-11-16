# 📊 Exploratory Data Analysis (EDA) - Superstore Sales Dataset
**Devixo Solutions — Data Science Internship Program | Task 01**

---

## 👤 Intern Information
* **Intern Name:** Abdul Rafay
* **Internship Domain:** Data Science
* **Task Number:** Task 01 – Exploratory Data Analysis (EDA)
* **GitHub Repository:** [RxNultra/Superstore-Sales-EDA-Internship](https://github.com/RxNultra/Superstore-Sales-EDA-Internship)

---

## 🚀 Project Overview
This project constitutes **Task 01** of the Devixo Solutions Data Science Internship. The objective is to perform a rigorous, end-to-end Exploratory Data Analysis (EDA) on a real-world retail dataset (`train.csv`) containing four years of United States retail transactions (2015–2018). Through Python-based data cleaning, statistical profiling, feature engineering, correlation modeling, and multi-dimensional visualizations, this study uncovers revenue drivers, customer purchasing behaviors, regional disparities, and seasonal demand trends.

---

## 📂 Repository Structure
Your complete GitHub submission repository contains the following files and directories:
```text
📦 Superstore-Sales-EDA-Internship/
│
├── 📜 README.md                  # Comprehensive project documentation (this file)
├── 📓 superstore_eda.ipynb       # Fully documented Jupyter Notebook with all code & outputs
├── 📊 train.csv                  # Raw Superstore Sales dataset (9,800 records)
├── 📄 EDA_Report.pdf             # Professional PDF report containing all structured findings & dashboards
└── 📁 screenshots/               # Directory containing code outputs, data cleaning checks & graph images
    ├── Capture.JPG               # Initial dataset loading and head/info logs
    ├── 1.JPG                     # Data cleaning verification & missing value imputation
    ├── 2.JPG                     # Statistical description and outlier metrics
    ├── 3.JPG                     # Categorical groupings and yearly sales aggregations
    ├── 4.JPG                     # Correlation heatmap
    ├── 5.JPG                     # Core revenue & growth dashboards
    └── 6.JPG                     # Seasonality, top states, and regional density charts
```

---

## 🗃️ Dataset Information
* **Dataset Name:** Superstore Sales Dataset (`train.csv`)
* **Source:** Kaggle (Retail Sales Dataset)
* **Total Records:** 9,800 transactions
* **Features:** 18 original columns (expanded to 21 columns after temporal feature engineering), covering transactional IDs, order/ship dates, customer segments, geographic regions, product hierarchies, fulfillment modes, and sales revenue.

---

## 🛠️ Technologies Used
* **Programming Language:** Python 3.12+
* **Libraries & Frameworks:**
  * `Pandas` & `NumPy` for data manipulation, cleaning, and statistical aggregations.
  * `Matplotlib` & `Seaborn` for advanced data visualization and correlation heatmaps.
  * `Jupyter Notebook` for interactive development and code execution.

---

## 🔍 Analysis Performed
1. **Data Import & Understanding:** Inspected dataset shape, data types, column names, head/tail records, and generated initial statistical summaries.
2. **Data Cleaning & Preparation:** Handled 11 missing values in `Postal Code` (imputed with `0`), verified zero duplicate records, standardized `Order Date` and `Ship Date` into `datetime64[ns]` objects, and engineered temporal features (`Shipping_Days`, `Order_Year`, `Order_Month`).
3. **Feature Analysis:** Analyzed univariate and grouped distributions across product categories (`Technology`, `Furniture`, `Office Supplies`), customer segments (`Consumer`, `Corporate`, `Home Office`), and geographic regions (`West`, `East`, `Central`, `South`), identifying high-value outliers ($> \$500.64$).
4. **Correlation Analysis:** Generated a Pearson correlation matrix and heatmap across numerical features, establishing that order sales have near-zero linear correlation with shipping days, order year/month, or postal codes.
5. **Data Visualization:** Built 13 analytical charts, including distribution plots, bar charts, line trends, correlation heatmaps, and regional violin plots.

---

## 💡 Key Findings & Business Insights (Summary)
* **Technology Revenue Leadership:** Technology generates **$827,455.87** in total revenue, outperforming Furniture ($728,658.58) and Office Supplies ($705,422.33).
* **High-Volume vs. High-Value Split:** Office Supplies accounts for **60.30%** of order volume but yields the lowest average order value ($119.38), whereas Technology commands an average of $456.40 per order.
* **Top Revenue Sub-Categories:** Phones and Chairs each exceed **$320,000** in sales, anchoring top-line company growth.
* **Skewed Basket Distribution:** The mean order value ($230.77) is over 4× higher than the median ($54.49), driven by 1,145 high-value corporate bulk orders (11.68% of the dataset).
* **Regional Concentration:** The West and East regions dominate with **61.01%** of total sales, while the South records the lowest order count (1,598) but the highest average order value ($243.52).
* **Q4 Seasonality Spikes:** Monthly sales trends reveal sharp, recurring demand surges in September, November, and December, peaking at over $722K in annual revenue for 2018.

---

## 🎯 Actionable Business Recommendations
1. **Cross-Sell Office Supplies with Technology:** Pair high-frequency Office Supplies (Binders, Paper) with Technology items (Phones, Accessories) via automated checkout bundles to lift average basket size.
2. **Launch Targeted B2B Volume Pricing:** Establish tiered discounts and dedicated account management for Corporate and Home Office buyers purchasing high-ticket items (Chairs, Tables, Copiers).
3. **Expand Marketing in the South Region:** Reallocate digital acquisition spend toward major metropolitan markets in the South to scale customer acquisition where per-order spend is highest ($243.52).
4. **Scale Q4 Logistics Capacity:** Increase safety stock for top sub-categories (Phones, Chairs, Storage) by late Q3 and pre-negotiate carrier capacity for Standard Class shipping to capture seasonal demand spikes.
5. **Implement Free Standard Shipping Threshold:** Introduce a "Free Standard Shipping on Orders Over $75" policy to incentivize median-tier shoppers (median = $54.49) to add extra items to their cart.

---

## ⚙️ Instructions to Run the Notebook
1. Clone the repository or download the project files:
   ```bash
   git clone https://github.com/RxNultra/Superstore-Sales-EDA-Internship.git
   cd Superstore-Sales-EDA-Internship
   ```
2. Ensure Python and Jupyter Notebook are installed along with required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Open Jupyter Notebook:
   ```bash
   jupyter notebook superstore_eda.ipynb
   ```
4. Run all cells sequentially to reproduce the data cleaning, statistical calculations, and visualizations.

---
*© 2016–2018 Devixo Solutions & Abdul Rafay. All rights reserved.*