# EDA and Linear Regression Model on Car Price Data

This repository contains an exploratory data analysis (EDA) and linear regression model to predict car prices based on various features.

## Overview

This project analyzes a car pricing dataset to understand the factors that influence car prices and builds a predictive linear regression model to estimate prices based on these factors.

## Dataset

The analysis uses a dataset (`car_price_prediction.csv`) containing information about various cars including:

- ID
- Price
- Levy
- Manufacturer
- Model
- Production year
- Category
- Leather interior
- Fuel type
- Engine volume
- Mileage
- Cylinders
- Gear box type
- And more

## Data Cleaning and Preprocessing

Before analysis, the data underwent thorough cleaning and preprocessing steps:
- Converting datetime variables to appropriate formats
- Normalizing numerical features where necessary
- Removing outliers that could skew the analysis

## Exploratory Data Analysis

Various graphs and visualizations were plotted to answer critical business questions:
- Distribution of car prices across different manufacturers/categories
- Relationship between mileage and price
- Impact of fuel type on pricing
- How production year affects car valuation
- Correlation between engine specifications and price points

These visualizations helped identify patterns and trends in the data that informed the subsequent modeling process.

## Key Findings

### Correlation Analysis

The correlation matrix reveals which features are most closely associated with price:
- Production year and Cylinders are slightly and positively correlated with Price
- Engine volume shows strong correlation with Cylinders (0.76)

### Hypothesis Testing

The project includes statistical tests such as:
- ANOVA test for price differences across fuel types (highly significant with p-value: 3.274e-244)

### Insights

- Higher cylinders generally correlate with higher prices, likely due to efficiency
- Leather interiors appear to increase price, suggesting they are viewed as a premium feature
- There is significant variation in price across fuel types, which could inform pricing strategies

### Recommendations

- For premium car segments, focus on models with leather interiors and larger engine volumes
- Consider expanding the selection of fuel-efficient or eco-friendly cars, given distinct pricing tiers by fuel type

## Predictive Modeling

The repository contains a linear regression model to predict car prices based on the following features:
- Production year
- Category
- Leather interior
- Fuel type
- Engine volume
- Mileage
- Cylinders
- And more

Categorical features are converted to numerical values using one-hot encoding.

## Implementation Details

- Data is split into training (80%) and testing (20%) sets
- The model is trained using scikit-learn's LinearRegression
- Predictions and evaluations are included in the notebook

## Technologies Used

- Python
- pandas for data manipulation
- NumPy for numerical operations
- Matplotlib/pyplot for visualization
- Seaborn for statistical visualizations
- scikit-learn for model training and evaluation

## Getting Started

1. Clone this repository
2. Ensure you have the required Python packages installed
3. Open the Jupyter notebook `EDA_RegressionModel.ipynb` to view the analysis and model

 **If you found this project helpful, please give it a star!** 
