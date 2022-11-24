
# Prediction of Absenteeism during work time: Project Overview 

* Business Problem: Currently the home loan application process is a manual one. It which takes 2-3 days, which mean that the applicant will only be notified after 2-3 days of the application outcome.

* Business Objective: Reduce the amount of time it takes for applicants to be notified about their loan statuses (to a matter of seconds).

Hypothesis: Based on historical data we can use machine learning to predict the loan status of a potential borrower such that the time taken for them to receive their respective statuses is reduced significantly.


* Created a tool that predicts absenteeism at a company during work time which will helpful to regulate working activity and also explore whether a person presenting certain characteristics is expected to be away from work at some point time or not.

* I have collected data from Kaggle in csv file, Pre-processed (Cleaning/ Analysis) data with Python & SQL, finally saved pre-processed data in csv file.
* Applied Feature Engineering, Logistic Regression (ML) with sklearn, obtained 73% accuracy, saved model using pickle
* Model deployed through absenteeism module and Analysed the Predicted Outputs in Tableau.

## Dataset:
This dataset is taken from Kaggle which is famous for it employment service and data has following features:
*	ID
*	Reason for Absence
*	Date
*	Transportation Expense
*	Distance to Work 
*	Age
*	Daily Work Load Average
*	Body Mass Index
*	Education
*	Children 
*	Pets
*	Absenteeism Time in Hours



## Data Cleaning
After collecting the data, I needed to clean it up so that it was usable for our model. I made the following changes and created the following variables:

*	Dropping unnecessary ID column from dataset
*	Created dummies for Reason for Absence column, later grouped and added into 4 category columns
*	Reordered the 4 reason columns like original dataset order
*	Converted date string data type to datetime datatype 
*	Made a new columns for Month value and Day of the week
*	And made many more changes which can be viewed in the pre-processed data csv

## Exploratory Data Analysis (EDA)
Performed EDA on the cleaned data and got various insights, relationships, etc, few of them are as below.

* There are total 700 rows and 14 columns after pre-processed data
* There are total 28 unique type of values presents in the Reason for absence column
* 4 types of values presents in the Education column, highest being the value 1


## Model Building 

First, I transformed the categorical variables into dummy variables, then scaled with standard scaler from sk-learn. I also split the data into train and tests sets with a test size of 20%.   

I tried Logistic Regression model and evaluated. 

I tried Logistic regression model:
*	**Logistic Regression** – for prediction of categorical outcomes, with the sparsity associated with the data, I thought that this would be a good fit.  

## Model performance
The Logistic Regression model performed good on the test and validation sets. 
*	**Logistic Regression** : 73%



## Productionization 
In this step, I saved the prepared model using pickle module for further deploymnet. Then Created a absenteeism_module for deployment.Finally, Analyzed the Predicted Outputs in Tableau for various variables.



## Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, sklearn, pickle

**The Data Science Course 2022: Complete Data Science Bootcamp**
https://www.udemy.com/course/the-data-science-course-complete-data-science-bootcamp/

**Ken Jee Youtube channel**
https://www.youtube.com/c/KenJee1







