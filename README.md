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
