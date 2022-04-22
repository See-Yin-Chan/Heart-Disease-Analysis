# Welcome to Heart-Disease-Analysis!

## Description
This is our mini project for the SC1015 Introduction to Data Science and Artificial Intelligence module. In this project, we used classification models to predict if an individual has heart disease. We utilised classification models because we wanted to identify different categories in the dataset and use these categories to make a prediction.

## Table of Contents
1. [Data Cleaning](https://github.com/See-Yin-Chan/Heart-Disease-Analysis/blob/6adb701a70ae569cb35d5c7125d16ce687da4565/Data%20Cleaning.ipynb)
2. [Data Visualisation and Analysis](https://github.com/See-Yin-Chan/Heart-Disease-Analysis/blob/6adb701a70ae569cb35d5c7125d16ce687da4565/Data%20Visualisation%20and%20Analysis.ipynb)
3. [Classification Models](https://github.com/See-Yin-Chan/Heart-Disease-Analysis/blob/6adb701a70ae569cb35d5c7125d16ce687da4565/Classification%20Models.ipynb)

## Problem Definition
* Can we predict whether a person has heart disease?
* Which classification model is the best at predicting whether a person has heart disease?

## Data Preparation
We decided to use the Cleveland dataset as it has the least missing values. We chose this data set because it allows us to solve the problem of predicting the presence of cardiac disease through supervised learning. This enables us to develop better models whose accuracy can be quantified. We replaced null values with the mode as the missing values were categorical variables. We performed mapping on multiple variables so that we could classify them.

## Exploratory Data Analysis
We created a series of heatmaps, barplots, histograms, violinplots, catplots to explore the relationships between two or more variables. We noticed that some relationships were out of the ordinary and thus explained our analysis in the notebook.

## Machine Learning
We utilised the following classification models:
1. Decision Trees
2. XGBoost
3. Logistic Regression

## Conclusion and Data Driven Insights
* We found that it is indeed possible to predict if an individual has heart disease.
* XGBoost was the best model to use in our case as it had the highest accuracy and F1 score.
* Surprisingly, we found that GridSearch might not increase the accuracy and F1 score. The usefulness of GridSearch is based on the parameters that we fit it with.
* Angiographic heart disease does not always cause chest pain as seen from how most of the patients were asymptomatic.
* An abnormal ECG does not immediately mean angiographic heart disease is present as seen by how there are many data points with ECG irregularities but are under DIS = 0. Abnormal heart behaviour can sometimes be explained by other conditions such as anaemia or lung diseases since they would also decrease oxygen flow to the heart. 

## Learning Something New
Through this project, we learnt how to:
* How to clean and prepare datasets, especially those with many categorical variables and few numerical variables
* Logistic Regression from sklearn for classification
* XGBoost from xgboost for classification
* Extracting information from trends and visuals statistics
* Creating a repository and collaborating on Github
* Differences between F1 and accuracy as evaluation metrics

## Applications of our Findings
* An application can be created using the best model we have identified. This application can be used to predict the likelihood of heart disease. Doctors can then warn patients and can enable early treatment.
* The impact on the likelihood of heart disease can be included. This helps doctors to raise awareness and showcase to others that there is a higher likelihood of disease if current lifestyle factors are unhealthy.

## Contributors
* See Yin - Data Preparation and Cleaning, Machine Learning (XGBoost), Presentation Slides and Script
* Jessica - Exploratory Data Analysis, Machine Learning (Logistic Regression), Presentation Slides and Script
* Kakuly - Exploratory Data Analysis, Machine Learning (Decision Trees), Presentation Slides and Script

## References
* http://scikit-learn.org/stable/modules/tree.html#:~:text=Decision%20Trees%20(DTs)%20are%20a,as%20a%20piecewise%20constant%20approximation.
* https://www.sciencedirect.com/topics/computer-science/logistic-regression#:~:text=Logistic%20regression%20is%20a%20process,%2Fno%2C%20and%20so%20on.
* https://machinelearningmastery.com/xgboost-for-regression/
* https://www.who.int/news-room/fact-sheets/detail/cardiovascular-diseases-(cvds)#:~:text=Cardiovascular%20diseases%20(CVDs)%20are%20the,%2D%20and%20middle%2Dincome%20countries. 
* https://towardsdatascience.com/the-f1-score-bec2bbc38aa6
* https://www.datacamp.com/community/tutorials/xgboost-in-python
* https://towardsdatascience.com/beginners-guide-to-xgboost-for-classification-problems-50f75aac5390
