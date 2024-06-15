# House Price Prediction using Linear Regression

## Overview

This project implements a Linear Regression model to predict the sale price of houses based on various features including square footage, number of bedrooms, and number of bathrooms. 

## Features

- **Outlier Handling**: The Interquartile Range (IQR) method is used to detect and handle outliers, ensuring the model's robustness and reliability.
- **Data Visualization**: Box plots are employed to visualize data distributions and highlight outliers.
- **Cross-Validation**: The KFold cross-validation method is used for training the model, which is particularly useful for dealing with skewed data distributions.

## Dependencies

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib (for visualization)

The description of the dataset is given in a file: data_description.txt

Ensure that your data is cleaned and preprocessed before running the model.

## Methodology

1. **Data Preprocessing**:
    - Handle missing values.
    - Normalize the features using MinMaxScaler.
    - Create new features as needed (e.g., house age from YearBuilt and YrSold).

2. **Outlier Detection**:
    - Use the IQR method to identify and handle outliers.

3. **Data Visualization**:
    - Use box plots to visualize the distribution of features and identify outliers.

4. **Model Training**:
    - Use KFold cross-validation to train the Linear Regression model and evaluate its performance.

5. **Model Evaluation**:
    - Calculate metrics such as Mean Squared Error (MSE) and R-squared (R²) to assess the model's accuracy.

## Results

The model achieves an average R-squared (R²) score of 0.8125 across 5 folds, indicating a good fit to the data.
