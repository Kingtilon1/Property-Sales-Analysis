# Property Sales Analysis

## Overview
This project analyzes property sales data from 2018 to 2022, exploring trends in property values over time. The analysis utilizes R for data manipulation, statistical testing, and visualization, including interaction with SQL and MongoDB databases to retrieve data.

## Repository Contents
- **Analysis Script**: The main R Markdown file containing all data analysis steps, from data fetching to statistical testing and visualization.
- **config.yaml**: Contains configuration settings for SQL database connections.
- **Data Files**: Includes links to property sales data for different years, stored in SQL and MongoDB databases.

## How to Run
To run this analysis, you will need R and RStudio installed on your computer, along with access to the SQL and MongoDB databases where the property sales data is stored.

### Setup
1. **Install R and RStudio**: Make sure you have R and RStudio installed. You can download them from [CRAN](https://cran.r-project.org/) and [RStudio's website](https://rstudio.com/products/rstudio/download/) respectively.
2. **Clone the Repository**: Download or clone this repository to your local machine.

### Dependencies
Before running the script, install the required R packages. You can do this by running the following commands in RStudio:
```r
install.packages("RMySQL")
install.packages("yaml")
install.packages("ggplot2")
install.packages("dplyr")
install.packages("tidyverse")
install.packages("infer")
install.packages("rvest")
install.packages("mongolite")
```
## Running the Analysis

To run this analysis, follow these steps:

### Setup Instructions
1. **Open the R Markdown File**: Open the R Markdown file (`property_sales_analysis.Rmd`) in RStudio.
2. **Configure Database Connections**:
   - **SQL Database**: Update the `config.yaml` file with the credentials for your SQL database.
   - **MongoDB Atlas**: Ensure that your MongoDB Atlas cluster is accessible and update the URI in the script if necessary.

### Execution
3. **Run the R Markdown File**: Click on "Knit" in RStudio to run the analysis and generate an HTML report, or run each code chunk sequentially using the "Run" button.

## Troubleshooting

If you encounter issues while running the analysis, consider the following troubleshooting steps:

### Database Connections
- If you have problems connecting to the SQL or MongoDB databases, check your firewall settings and ensure that your database credentials are correct.

### Package Errors
- Make sure all required R packages are installed and up-to-date. If you encounter errors related to missing or outdated packages, you can install or update them using the command `install.packages("package_name")` or `update.packages()` in R.

## Key Findings and Conclusions

### Price Fluctuations
From 2018 to 2022, the property sales data exhibited significant price fluctuations:
- A notable increase in average prices was observed from 2018 to 2019.
- This was followed by a decrease in 2020.
- Steady rises in average sale prices were noted in the years 2021 and 2022.

### Statistical Analysis
- **Linear Regression Model**: The linear regression analysis indicated a statistically significant upward trend in average sale prices over the years. This was supported by very low p-values (less than 0.001) for the coefficients associated with each year, indicating strong statistical significance.

### Model Effectiveness
- **R-squared Values**: The high R-squared values, close to 1, suggest that the linear regression model was highly effective in explaining the variance in sale prices based on the year. This confirms the hypothesis of a consistent increase in property values.

### Geospatial Insights
- **Mapping Property Locations**: Visualization of property locations using Google Maps API provided geographical insights into the data, enhancing the analysis with spatial distribution patterns. The maps helped illustrate where properties are concentrated and highlighted potential areas of interest for further real estate development or investment.

### Hypothesis Testing
- **Commercial Property Analysis**: Hypothesis testing between commercial property sale prices in 2020 and 2021 showed no significant difference, as indicated by the p-value of the t-test. This suggests that, at least for commercial properties, the year did not significantly impact sale prices.

## Conclusion
This comprehensive analysis of property sales trends from 2018 to 2022 employed advanced statistical techniques and geospatial visualization to draw meaningful insights into the dynamics of real estate markets. The findings suggest a general upward trend in property values, with year-to-year fluctuations providing deeper insights into market behavior under varying economic conditions. These results are crucial for stakeholders in making informed decisions in the real estate market.

