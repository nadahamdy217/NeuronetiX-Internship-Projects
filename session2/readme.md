# Financial Data Analysis

## Overview
This repository contains a comprehensive analysis of financial data related to various products across different countries. The analysis involves data cleaning, outlier detection, normalization, and visualization of key metrics such as Profit, Sales, and COGS.

## Table of Contents
- [Installation](#installation)
- [Data Description](#data-description)
- [Data Cleaning](#data-cleaning)
- [Outlier Detection](#outlier-detection)
- [Data Normalization](#data-normalization)
- [Data Visualization](#data-visualization)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)

## Installation
To run this analysis, ensure you have Python installed. Then, install the required libraries by running:

```
pip install pandas numpy matplotlib
```

## Data Description
The dataset consists of the following columns:

| Column               | Description                                               |
|----------------------|-----------------------------------------------------------|
| Segment              | Market segment of the product                             |
| Country              | Country where the product is sold                         |
| Product              | Name of the product                                       |
| DiscountBand         | The discount band applied to the product                  |
| UnitsSold            | Number of units sold                                      |
| ManufacturingPrice   | Price of manufacturing the product                        |
| SalePrice            | Selling price of the product                              |
| GrossSales           | Total gross sales amount                                  |
| Discounts            | Total discounts applied                                   |
| Sales                | Net sales amount                                         |
| COGS                 | Cost of Goods Sold                                       |
| Profit               | Profit earned from sales                                  |
| Date                 | Date of the transaction                                   |
| MonthNumber          | Month number of the transaction                           |
| MonthName            | Month name of the transaction                             |
| Year                 | Year of the transaction                                   |


## Data Cleaning
The following steps were performed during data cleaning:

1. **Check for Null Values** - The dataset was checked for any missing values.
2. **Convert Columns to Numeric** - Invalid values in the numeric columns were coerced to NaN.
3. **Handle Null Values** - 
   - The `DiscountBand` column was filled with the mode of the column.
   - The `Profit` column was filled with the median of the column.
4. **Check for Duplicates** - The dataset was checked for any duplicate entries.
5. **Replace Invalid Values** - Invalid values such as `'-'` were replaced with `0`, and `-1` values were replaced with median values.

## Outlier Detection
Outliers in the dataset were detected and handled using the Interquartile Range (IQR) method.

## Data Normalization
Min-Max normalization was applied to the relevant columns to scale the data between `0` and `1`.

## Data Visualization
The analysis includes a stacked bar chart representing Profit, Sales, and COGS across different countries.

### Stacked Bar Chart
(![Stacked Bar Chart](https://github.com/user-attachments/assets/0a18c2c9-c4bf-4bdd-9e04-7a907902e197)
)

### Additional Visualizations
Additional visualizations may be included as needed.

## Results
The analysis provides insights into:
- The performance of different segments across various metrics.
- The impact of discounts on sales and profit.

## Usage
To run the analysis, open the Jupyter Notebook and execute the code cells sequentially. Ensure that the path to the CSV file is correctly set in the code.

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.
