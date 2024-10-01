# BoomBikes Regression Project

### Author: Devesh Kumar

## Project Overview

This project aims to build a linear regression model to predict the demand for shared bikes at BoomBikes, a US-based bike-sharing service provider. The company is experiencing revenue challenges due to the pandemic and is looking to prepare for post-pandemic demand. By understanding the factors that influence bike demand, BoomBikes hopes to adapt its business strategy and gain a competitive edge.

## Business Goal

BoomBikes wants to:
- Identify the variables that significantly impact the demand for shared bikes.
- Develop a model to predict bike demand based on these variables.

This model will help BoomBikes anticipate demand, adjust operations accordingly, and maximize revenue in the post-lockdown era.

## Dataset

The dataset used in this project contains daily bike demand data, along with factors such as weather, season, and user types (casual vs. registered). The target variable is `cnt`, which represents the total number of bike rentals.

### Features:
- `instant`: record index
- `dteday`: date
- `season`: season (1: spring, 2: summer, 3: fall, 4: winter)
- `yr`: year (0: 2018, 1: 2019)
- `mnth`: month (1 to 12)
- `holiday`: whether the day is a holiday (0: No, 1: Yes)
- `weekday`: day of the week (0 to 6)
- `workingday`: whether the day is a working day (0: No, 1: Yes)
- `weathersit`: weather situation (1: Clear, 2: Mist, 3: Light Snow/Rain, 4: Heavy Rain/Snow)
- `temp`: temperature in Celsius
- `atemp`: "feeling" temperature in Celsius
- `hum`: humidity
- `windspeed`: wind speed
- `casual`: number of casual users
- `registered`: number of registered users
- `cnt`: total number of bike rentals

## Data Preparation

Before building the model, the dataset was cleaned and processed:
- Checked for missing values, and no missing data was found.
- Converted some features like `season`, `yr`, `mnth`, `holiday`, `weekday`, `workingday`, and `weathersit` from numerical to categorical data.
- Generated visualizations to better understand the distribution and relationships in the data.

## Model Building

A linear regression model was built with the following steps:
1. Data splitting: The dataset was split into training and test sets.
2. Feature selection: Key features influencing demand were identified.
3. Model training: A linear regression model was trained on the training set.
4. Evaluation: The model was evaluated using R-squared scores and residual analysis.

## Model Evaluation

The model's performance was evaluated using the R-squared score, which indicates how well the independent variables explain the variance in bike demand.


## Results

R-squared score: 0.8622. The residuals were also checked for normality using histograms and QQ plots to ensure that the model assumptions were met.

## Conclusion

The linear regression model explains about 86% of the variance in bike demand based on the features in the dataset. This model will help BoomBikes predict demand more accurately and improve their business strategy as they prepare for post-pandemic recovery.

## Repository Structure

- `BoomBikes_Regression_Project.ipynb`: Jupyter notebook containing the entire project.
- `day.csv`: The dataset used for analysis and model building.
- `README.md`: This file.
- `subjective_answers.pdf`: A PDF file containing all subjective answers.
