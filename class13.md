# How to Run Linear Regression in Python

Linear regression uses the relationship between the data-points to draw a straight line through all them.This line can be used to predict future values.

## Scikit Learn

functions to keep in mind while fitting a linear regression model are:

lm.fit() -> fits a linear model

lm.predict() -> Predict Y using the linear model with estimated coefficients

lm.score() -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.

You can also explore the functions inside lm object by pressing lm.<tab>

## Fitting a Linear Model

In [20]: lm.fit(X, bos.PRICE)

Out[20]: LinearRegression(copy_X=True, fit_intercept=True, normalize=False)

## Training and validation data sets

create training and test data sets manually, but this is not the right way to do, because you may be training your model on less expensive houses and testing on expensive houses.



