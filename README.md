# Project Name
> Building a multiple linear regression model for the prediction of demand for shared bikes

## Table of Contents
* [Problem Statement](#problem-statement)
* [Business Goal](#business-goal)
* [Steps taken to build a model](#steps-taken-to-build-a-model)
* [Packages Used](#packages-used)
* [Conclusions](#conclusions)
* [Contact](#contact)

## Problem Statement

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.


A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 


In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.


They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 

## Business Goal:

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 


## Steps taken to build a model
1) Reading and Understanding the Data
2) Visualizing the data
3) Preparing the data
4) Splitting the data in training and test data set
5) Building a linear model
6) Residual analysis of the train data
7) Making Predictions Using the Final Model
8) Model Evaluation


## Packages used
import warnings
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import sklearn as sk
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import MinMaxScaler
from sklearn.feature_selection import RFE
from sklearn.linear_model import LinearRegression
import statsmodels.api as sm
from statsmodels.stats.outliers_influence import variance_inflation_factor
from sklearn.metrics import r2_score

## Conclusions
- We can see that the equation of our best fitted line is:

cnt = 0.1868\
    + (temp * 0.5158)\
    + (windspeed * -0.1532)\
    + (winter * 0.0879)\
    + (2019 * 0.2345)\
    + (jan * -0.0819)\
    + (sep * 0.069)\
    + (sun * -0.0473)\
    + (light_now * -0.0473)\
    + (mist * -0.0736)

- R2 score: 0.7675344746595867


## Contact
Created by [@Rishabh-Saha] - feel free to contact me!


