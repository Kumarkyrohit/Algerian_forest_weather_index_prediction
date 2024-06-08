# Algerian Forest Fires Analysis

## Project Overview

This project involves the analysis and modeling of the Algerian Forest Fires dataset to predict forest fire occurrences and their severity. The project is divided into the following sections:
1. Data Cleaning and Preprocessing
2. Data Visualization and Observations
3. Checking for Multicollinearity
4. Model Development and Analysis
5. Model Evaluation and Testing
6. Model Saving and Loading

## Dataset

The dataset used in this project contains the following columns:
- `day`: Day of the month
- `month`: Month of the year
- `year`: Year
- `Temperature`: Temperature in Celsius
- `RH`: Relative Humidity
- `Ws`: Wind speed in km/h
- `Rain`: Rain in mm/m2
- `FFMC`: Fine Fuel Moisture Code
- `DMC`: Duff Moisture Code
- `DC`: Drought Code
- `ISI`: Initial Spread Index
- `BUI`: Buildup Index
- `FWI`: Fire Weather Index
- `Classes`: Fire classes (1 for fire, 0 for no fire)
- `Region`: Region of the observation

## Data Cleaning and Preprocessing

1. Handling missing values.
2. Removing irrelevant features.
3. Encoding categorical variables.
4. Normalizing/standardizing numerical features.

## Data Visualization and Observations

### Univariate Plots

Univariate plots were created to understand the distribution of individual features.

### Bivariate Plots

Bivariate plots were created to understand the relationships between pairs of variables. This includes:
- Scatter plots of each numerical feature against the target variable `FWI`.
- Correlation matrix to check for multicollinearity among features.

## Checking for Multicollinearity

Variance Inflation Factor (VIF) was used to detect multicollinearity among the features. Features with a high VIF value were considered for removal.

## Model Development and Analysis

### Models Used

1. Linear Regression
2. Polynomial Regression
3. Ridge Regression
4. Lasso Regression
5. Decision Tree Regression

### Hyperparameter Tuning

GridSearchCV was used to find the best model and best parameters from all the model. The best model selected was Decision Tree Regression with the following parameters:
- `max_depth`: 10

## Conclusion
This project demonstrates the process of data cleaning, preprocessing, visualization, model development, and evaluation to predict forest fire occurrences and their severity using the Algerian Forest Fires dataset. The Decision Tree Regression model was found to be the best performing model, and it was saved for future use.