## Introduction

### Project 06 - Linear Regression

This is a project to train a machine learning model to predict healthy life expectancy based on data from the World Happiness Data Csv in this folder.

The Features are GDP per capita, Generosity score, Social support score, Perceptions of corruption score, and Freedom to make life choices score. 

Happiness ranking is based on "Ladder Score".  This was taken from a Gallup poll where individuals were asked to rank their happiness as if it were rungs on a ladder.  The happier they were the Higher the score.  Other features were added to the data set to determine if these played a factor in how happy the people considered themselves.  

### Model

We will attempt to build a linear regression model that will predict a happiness/Ladder score based on input of several features.  


There are 140 rows of data each representing one country.  The numerical data includes a score or number that is a calculation of the feature. For example the perception of corruption is a number that if its higher it implies that people percieve their country to be corrupt.   Similarly, if the social support number is low then there must not be a good welfare system and perhaps more poverty.   Other features such as Healthy life expectency are straight forward indiciting the average age of people in the country.  For training the model we will not use "Ranking" or Region as they are not going to be a factor in traininig the model.  

The notebook can be found here:
[https://github.com/nwn8/applied-ml-nates/blob/main/notebooks/project06/ml_regression_NathanSloss.ipynb]