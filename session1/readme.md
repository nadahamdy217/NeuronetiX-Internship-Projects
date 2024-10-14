# Transactional Data Analysis: Insights into Customer Behavior and Sales Trends

## Overview
This repository contains a comprehensive analysis of fitness-related data, focusing on key metrics such as Duration, Pulse, Maxpulse, and Calories. The analysis is conducted using Python libraries including Pandas, Seaborn, and Matplotlib to visualize data and uncover insights.

## Dataset
The dataset includes the following columns:
- **Duration**: Duration of the activity (in minutes).
- **Pulse**: Average pulse rate during the activity.
- **Maxpulse**: Maximum pulse rate during the activity.
- **Calories**: Total calories burned during the activity.

## Tools Used
- **Python**: Main programming language for data analysis.
- **Pandas**: Library for data manipulation and analysis.
- **Seaborn**: Library for statistical data visualization.
- **Matplotlib**: Library for creating static, animated, and interactive visualizations.

## Install the Required Libraries
To install the required libraries, run the following command in your terminal:

```
pip install pandas seaborn matplotlib
```

## Data Analysis
The following steps are included in the analysis:

### Loading Data
- Data is loaded from a CSV file using Pandas.

### Data Cleaning
- Missing values in the 'Calories' column are filled with the average value.
- Duplicate rows are identified and removed.
- Outliers in the 'Calories', 'Duration', 'Pulse', and 'Maxpulse' columns are detected and replaced with the mean value.

### Data Visualization
- Box plots to identify and visualize outliers.
- Line plots showing the relationship between Duration and other metrics (Pulse, Maxpulse, and Calories).
- Histograms visualizing the distribution of Pulse, Maxpulse, and Calories.
- Bar plot displaying the average values of these metrics.
- Heatmap illustrating the correlation matrix between the variables.

## Results
The analysis provides insights into:
- The relationship between activity duration and heart rate.
![image](https://github.com/user-attachments/assets/b9aa28bb-e308-49ca-8f01-834fdf1197c3)

- The distribution of calories burned across different activities.
![image](https://github.com/user-attachments/assets/cfa8ada0-c8c6-4eaf-b5bb-5b6813907712)

- Correlations between pulse metrics and calorie expenditure.
![image](https://github.com/user-attachments/assets/52138266-4e27-4ce6-84ac-5e72fadb3776)


## Usage
To run the analysis, open the `data_analysis.ipynb` Jupyter Notebook and execute the code cells sequentially. Make sure to update the path to the CSV file if needed.

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.
