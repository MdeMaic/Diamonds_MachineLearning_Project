# Daimonds Machine Learning | Project

## Objective
Create the best regression model of machine learning that can predict the price (independent variable) of the diamonds when a certain characteristic (features) are given. 

## Instrucctions
Two datasets are given in a [kaggle competition](https://www.kaggle.com/c/diamonds-datamad0120)

- Train Set: with the following columns. 

| Feature | Description |
| --- | --- |
|`id` | only for test & sample submission files, id for prediction sample identification |
|`carat`| weight of the diamond |
|`cut`| quality of the cut (Fair, Good, Very Good, Premium, Ideal) |
|`color`| diamond colour, from J (worst) to D (best) |
|`clarity`| a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best)) |
|`x`| length in mm |
|`y`| width in mm |
|`z`| depth in mm |
|`depth`| total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79) |
|`table`| width of top of diamond relative to widest point (43--95) |

| Independent variable | Description |
| --- | --- |
|`price` | price in USD |

- Test Set: With the same features of the training set but in this case without the price, that has to be predicted using the ML model. 

- Submit Set: Id the test set with the only columns of “id” and “price”. This set has to be submitted to Kaggle competition that will return a score based on the MRSE. The lower this score, the better model you are delivering. 

## Resources and libraries
- Sklearn | Machine Learning Library with regression models
- TensorFlow Keras | ML library
- h2O | Auto ML module for machine learning

## Inputs
- diamonds_train.CSV | Shape (40345, 11)
- diamonds_test.CSV | Shape (13449, 10)

## Outputs
- Models submitted to the kaggle competition
- Jupyter Notebooks of the process of each model

## Methodology
1. Cleaning Dataset
The following decision has to be done 
    - Ensure not Null values
    - Avoid not numeric values
    - Drop the high correlated features
    - Standarize or normalize high value range features

2. Identify the best model
Different models apport different results. Some of them are analysed in the project.
    - LinearRegression
    - RandomForestRegression
    - LassoCV
    - SGDRegressor
    - Keras Sequential
    - SVR
    - Polynomic RFR
    - Sum of two Polynomic RFR

3. Analyse the result
There are metrics from sklearn that help you to choose the best model
    - R2_score
    - MRSE
    - Scatter plot y_test vs y_true

## Results

![Result table](/outputs/img/results.png)