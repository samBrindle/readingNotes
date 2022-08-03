# Reading 13 - Linear Regressions
## How to run Linear Regression in Python scikit learn
* Sciki-learn is a powerful Python module for machine learning
  * It contains regression, classification, clustering, model selection and dimensionality reduction

## Scikit Learn
* Make a y axis
* Make a x axis
* Important Functions while fitting a linear regression model:
  * lm.fit() -> fits a linear model
  * lm.predict() -> Predict Y using the linear model with estimated coefficients
  * lm.score() -> Returns the coefficient of determination. A measure of how well observed outcomes are replicated by the model, as the proortion of total variation of outcomes explained by the model
  * lm.coef_ -> Estimated coefficients
  * lm.intercept_ -> Estimated intercept

## Training and validation data sets
* You need to split the data sets into training and test data sets
* You should not create these test data sets manually

## How to do train-test split
* You need to divide your data sets randomly
* Use scikit learns functino called `train_test_split`

## Residual Plots
* Good Job - Data is randomly scattered around line zero
* Not Capturing something - Structure in the data
