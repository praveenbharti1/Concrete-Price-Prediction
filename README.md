# Predicting Concrete Strength

This project aims to predict the future strength of a concrete mix, based on its constituents’ composition and also the age of the mix. It uses various machine learning algorithms to build and evaluate regression models on a dataset of concrete samples.

## Data Analysis

The dataset contains 1030 instances of concrete samples, with 9 attributes: cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, fine aggregate, age, and concrete compressive strength. The dataset can be found [here](^1^).

The data analysis process involved the following steps:

- Removing duplicate data points from the dataset
- Detecting and imputing outliers using the interquartile range (IQR) method
- Handling zero values in the slag, ash, and superplasticizer columns using the KNN imputer
- Applying log transformation to the independent features to improve their distribution
- Scaling the data using the standard scaler

## Model Creation

The model creation process involved the following steps:

- Splitting the data into train and test sets
- Applying various regression algorithms to the train set and evaluating their performance on the test set using metrics such as mean absolute error (MAE), root mean squared error (RMSE), and coefficient of determination (R2)
- Comparing the results of different algorithms and selecting the top three models
- Performing hyperparameter tuning on the top three models using grid search and cross-validation
- Choosing the best model based on the tuned performance

The regression algorithms used in this project are:

- Linear Regression
- Ridge Regression
- Lasso Regression
- ElasticNet Regression
- Support Vector Regression
- Decision Tree Regression
- Random Forest Regression
- K-Nearest Neighbor Regression
- XGBoost Regression
- Gradient Boosting Regression
- AdaBoost Regression

The top three models based on the initial performance are:

- Gradient Boosting Regression
- XGBoost Regression
- Decision Tree Regression

The best model based on the tuned performance is:

- XGBoost Regression

## Conclusion

The project demonstrates how to use machine learning to predict the concrete strength based on the mix composition and age. The best model for this task is the XGBoost regression model, which achieved a MAE of 2.32, a RMSE of 3.18, and an R2 of 0.93 on the test set. This model can be used for production to predict the future strength of a concrete mix..

