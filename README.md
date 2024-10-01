# BoomBikes Regression Project

### Author: Devesh Kumar

## Project Overview

This project aims to build a linear regression model to predict the demand for shared bikes at BoomBikes, a US-based bike-sharing service provider. The company is experiencing revenue challenges due to the pandemic and is looking to prepare for post-pandemic demand. By understanding the factors that influence bike demand, BoomBikes hopes to adapt its business strategy and gain a competitive edge.

## Table of Contents
* [Project Overview](#project-overview)
* [Business Goal](#business-goal)
* [Data Preparation](#data-preparation)
* [Model Building](#model-building)
* [Model Evaluation](#model-evaluation)
* [Results](#results)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Repository Structure](#repository-structure)
* [Contact](#contact)

## Business Goal

BoomBikes wants to:
- Identify the variables that significantly impact the demand for shared bikes.
- Develop a model to predict bike demand based on these variables.

This model will help BoomBikes anticipate demand, adjust operations accordingly, and maximize revenue in the post-lockdown era.

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

## Conclusions
- The linear regression model explains approximately 86% of the variance in bike demand based on independent variables, indicating a strong relationship between the features and bike rentals.
- Significant factors affecting bike demand include temperature, weather situation, and seasonal effects.
- The model's predictions will assist BoomBikes in effectively planning for changes in customer demand.
- Understanding demand dynamics will enable BoomBikes to enhance customer satisfaction and increase profitability.

## Technologies Used
- pandas - version 1.3.3
- numpy - version 1.21.2
- matplotlib - version 3.4.3
- seaborn - version 0.11.2
- scikit-learn - version 0.24.2 

## Repository Structure

- `BoomBikes_Regression_Project.ipynb`: Jupyter notebook containing the entire project.
- `day.csv`: The dataset used for analysis and model building.
- `README.md`: This file.
- `subjective_answers.pdf`: A PDF file containing all subjective answers.

## Contact

Created by [@devesh0024](https://github.com/devesh0024) - feel free to contact me!
