# Retail Sales Exploratory Data Analysis

Exploratory data analysis of retail sales transactions from January 2023 through June 2025. The main analysis is in `DataAnalytics-L1-EDARetailSales/notebooks/Retail_Sales_EDA.ipynb`.

## Project Overview

This project examines sales performance, customer demographics, product revenue, seasonality, profitability, and discounting behavior. It is designed to turn transaction-level retail data into practical business recommendations.

## Project Structure

```text
DataAnalytics-L1-EDARetailSales/
├── data/
│   └── retail_sales_data.csv
├── notebooks/
│    └── Retail_Sales_EDA.ipynb
│── screenshots/
│   ├── Corr_Heatmap.png
│   ├── Customer_Age_Group_Segmentation.png
│   ├── Customer_Demographic.png
│   ├── Numerical_Variables_Distributions.png
│   ├── Revenue_by_Product_Category.png
│   ├── Sales_Time_Series.png
│   ├── Spread_Outliers.png
│   ├── Top_10_Products.png
│   └── Total_sales_and_Avg_ProfitMargin.png
└── README.md
```

## Outputs

The `screenshots/` directory stores the visual artifacts generated during the analysis:

- `Numerical_Variables_Distributions.png` — distributions of the main numerical variables
- `Spread_Outliers.png` — boxplots for sales, profit, and profit margin
- `Sales_Time_Series.png` — monthly and quarterly sales trends
- `Customer_Demographic.png` — age distribution and gender breakdown
- `Customer_Age_Group_Segmentation.png` — business-friendly age-group segmentation
- `Top_10_Products.png` — top 10 products ranked by total revenue
- `Revenue_by_Product_Category.png` — revenue comparison by product category
- `Corr_Heatmap.png` — correlations among numerical variables
- `Total_sales_and_Avg_ProfitMargin.png` — weekday sales and average profit margin

## Dataset

The dataset contains transaction-level records with fields including:

- Order and customer identifiers
- Order date, region, city, and customer segment
- Age and gender
- Product category, sub-category, and product name
- Unit price, quantity, discount, sales, and profit

The notebook creates additional fields for year, month, month period, quarter, day of week, profit margin, and business-friendly age group.

## Notebook Analysis

The notebook includes:

1. Data loading, inspection, and missing-value review
2. Descriptive statistics and distribution plots
3. Monthly and quarterly sales trends
4. Customer age distribution and gender breakdown
5. Age-group segmentation with customer count, sales share, average sales, and total sales
6. Top 10 products ranked by total revenue
7. Revenue analysis by product category
8. Correlation heatmap for numerical variables
9. Sales volume, discounting, and average profit margin by day of week
10. Conclusions and business recommendations

## Key Findings

- Sales show strong seasonality, with November and December as the strongest months and Q4 as the strongest quarter.
- Electronics generates approximately 56.1% of total revenue and contains all top 10 products by revenue.
- Smartphones - Model D is the highest-revenue product at approximately $417 thousand.
- Customers aged 35-44 are the largest age segment and generate the highest total sales.
- Apparel has the highest unit volume, but its lower average transaction value results in a smaller revenue share.
- Saturday and Sunday generate the highest sales volume, while average profit margin remains stable across the week at approximately 31%.
- Discounts have a strong negative relationship with profit margin but only a weak relationship with total sales.
- Unit price is more strongly related to sales and profit than quantity is, indicating the importance of higher-value products.

## Business Recommendations

- Protect inventory availability for leading Electronics products and use bundles or accessories to increase basket value.
- Prepare inventory, staffing, and marketing capacity ahead of the October-December peak.
- Use targeted January-February promotions and retention campaigns to reduce the post-holiday slowdown.
- Prioritize the 25-44 customer segments with personalized recommendations and loyalty campaigns.
- Test premium product lines, bundling, and selective price optimization in high-volume, lower-value categories such as Apparel.
- Strengthen staffing and service capacity from Friday through Sunday, and use targeted promotions on Monday and Tuesday.
- Replace broad discounting with targeted offers that protect profit margin.
- Monitor revenue, absolute profit, margin, discount rate, product availability, and customer retention together.

## Requirements

The notebook uses Python with the following packages:

- Python 3.10 or later
- pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook or VS Code with the Jupyter extension

## Running the Notebook

From the repository root, activate the project environment and launch Jupyter:

```powershell
.\Scripts\Activate.ps1
jupyter notebook
```

Then open:

```text
DataAnalytics-L1-EDARetailSales/notebooks/Retail_Sales_EDA.ipynb
```

Run the notebook cells from top to bottom. The notebook expects the CSV at:

```text
DataAnalytics-L1-EDARetailSales/data/retail_sales_data.csv
```

The notebook uses a relative data path, so it should be run with the notebook's project folder as the working context when necessary.
