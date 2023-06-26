# Boston House Price Prediction

This repository contains a multivariable regression model used to predict house prices in Boston in the 1970s. The model is implemented in a Jupyter Notebook using Python.

## Dataset
The dataset used for training and testing the model is stored in the file `boston.csv`. It contains information about various factors that can influence house prices, such as crime rate, zoning, industry, accessibility to highways, and more.

The dataset has the following columns:
- CRIM: per capita crime rate by town
- ZN: proportion of residential land zoned for lots over 25,000 sq.ft.
- INDUS: proportion of non-retail business acres per town
- CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
- NOX: nitric oxides concentration (parts per 10 million)
- RM: average number of rooms per dwelling
- AGE: proportion of owner-occupied units built prior to 1940
- DIS: weighted distances to five Boston employment centers
- RAD: index of accessibility to radial highways
- TAX: full-value property-tax rate per $10,000
- PTRATIO: pupil-teacher ratio by town
- B: 1000(Bk - 0.63)^2 where Bk is the proportion of Black people by town
- LSTAT: % lower status of the population
- PRICE: median value of owner-occupied homes in $1000s

## Model Training and Evaluation
The notebook contains the code for the following steps:

1. Importing necessary libraries and modules for data manipulation and modeling.
2. Data exploration using Pandas dataframes to gain insights into the dataset.
3. Cleaning the data by checking for missing values and handling duplicates.
4. Visualizing the data through histograms, distributions, and bar charts.
5. Calculating correlations between different features and the target variable.
6. Building and training a multivariable regression model using the LinearRegression class from scikit-learn.
7. Evaluating the model's performance by calculating the coefficient of determination (R-squared) and plotting the predicted prices against the actual prices.

## Results
The trained model achieves a coefficient of determination (R-squared) of approximately 0.695 when predicting house prices based on the average number of rooms (RM). The negative correlation between house prices and pupil-teacher ratio (PTRATIO) is approximately -0.508.

## Acknowledgments
The dataset used in this project is publicly available and can be found in the UCI Machine Learning Repository. The original source of the dataset is from the StatLib library maintained at Carnegie Mellon University.
