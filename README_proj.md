# Project 2: Ames Housing Linear Regression

## Problem Statement

You are tasked with creating a regression model based on the Ames Housing Dataset. This model will predict the price of a house at sale.

The Ames Housing Dataset is an exceptionally detailed and robust dataset with over 70 columns of different features relating to houses.

The Modeling Process The train dataset has all of the columns that you will need to generate and refine your models. The test dataset has all of those columns except for the target that you are trying to predict in your Regression model.

---

## Executive Summary


### Contents:
- [Data Cleaning](#data_cleaning)
- [Getting dummies](#get_dummies)
- [Add new variables](#new_variables)
- [Removing outliers and selecting features](#remove_outliers)
- [Preprocessing](#preprocessing)
- [Train-test-split and Scoring](#train_test_split)
- [Scoring with holdout set](#scoring_holdout)
- [Inferential Visualization](#visual_inference)
- [Business Recommendations](#business_recommendations)
- [Clean test and predict values](#clean_test_predict)

---

## Data Dictionary

Link to [Data Dictionary](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)

---

## Conclusions and Recommendations

The regression model of our choice is the Ridge model as it has the best Root Mean Squared Error for both the Train and Holdout set. (29359.60 and 31957.06 respectively) among the other regression models. Ridge model performs the best by shrinking the variable features and reducing multicollinearity. The model will perform best for housing in the 100k to 300k Sale Price range. However the model will not generalize to the prices of other cities as it is highly correlated to the Neighborhoods in Ames. 

Ground Living Area adds the most value to a home price. As the coefficient from the Ridge model is the highest. While age hurts the value of a home the most as the coefficient is the lowest from the Ridge model.

Homeowners should increase the Ground Living Area / overall material and finish of their homes to increase the Sale Price. However this is unlikely to be helpful as the construction/renovation cost could outweigh the increase in value. 

Some ways to increase the value of the home without construction/renovation related cost is to improve the Neighborhood conditions by requesting the Mayor of the Neighborhood to build more infrastructures and ameneties. 

Neighborhoods that might be a good investment are Stone Brook and Northridge Heights. They have the highest median sale price (300k and above) and also a concentrated range from 200k to 400k. Investing in these Neighborhoods have a higher probability than the rest of the Neighborhood to be sold at a price above 200k.
