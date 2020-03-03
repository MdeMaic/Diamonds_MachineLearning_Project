# Daimonds Machine Learning | Project

## OBJETIVE
Create the best regression model of machine learning that can predict the price (independent variable) of the diamonds when a certain characteristic (features) are given. 

## INSTRUCTIONS
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

## RESOURCES and LIBRARIES
- Sklearn | Machine Learning Library with regression models
- TensorFlow Keras | ML library
- h2O | Auto ML module for machine learning

## INPUTS
- diamonds_train.CSV | Shape (40345, 11)
- diamonds_test.CSV | Shape (13449, 10)

## OUTPUTS
- Models submitted to the kaggle competition
- Jupyter Notebooks of the process of each model

## METHODOLOGY
