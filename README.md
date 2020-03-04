# Predicting-Housing-Prices
Public Repo of my machine learning project to predict home prices
## Project Overview

The goal of this project is to predict the selling price of a home in Ames, Iowa, given certain the presence of certain features or characteristics in that home. 

There are many practical uses of a model such as this. For example, a home builder can identify the optimal number of bedrooms or bathrooms or a desirable neighborhood when building a new home to maximize selling price. A home owner could use this model to determine an optimal asking price for their home. Alternatively, a lender can look use the model to determine a home's value and use this to make loans or determine interest rates.

## EDA and Data Cleaning

The original dataset used for this analysis comes from the 'train.csv' file attached in the directory, which includes 80+ columns and more than 2,000 rows of data.

To create a successful model signifianct exploratory data analysis was required, including identifying outliers, determining appropriate treatment of missing values. Further EDA efforts included identifying numerical columns that had a relationship with our target variable, sale price. 

Additional EDA identified object columns that included categorical or ordinal information that could be converted to numerical amounts using feature engineering--identifying additional variables that are related to the target variable.

## Overall Findings

Using features that bear a correlation to the target, we can create use OLS regression to produce a model with strong predictive power. Employment of regularization techniques (Ridge and Lasso) to the OLS model improves predictive power of the model.

Using train/test split and cross validation score, I was able to train and test my model on different portions of the data set and evaluate whether my model suffers from high variance and can generalize well to new data. 

Regularization techniques including Ridge, apply a penalty to the loss function (SSE) to avoid overfitting the model—ensuring coefficients do not get too large-–ensuring coeffs are based on signal (what we want to detect and understand) and not noise.


## Conclusion

Generated a strong predictive model based on thorough exploratory data analysis, feature engineering and regularization of linear regression methods.

Overall R2 score (using ridge regression) indicates that ~ 89.5% of the variance in the Y holdout set is explained by our feature(s) relative to our predictions. 

To increase Sale Price of a home in Ames,  the most important feature to focus on is the overall quality score, along with ensuring the living area has a sufficient amount of square footage and the home is equipped with central air! 
