# Quantium Data Analytics Virtual Experience Program Overview 

* Prepared Customer analytics on given client's transaction dataset and identified customer purchasing behaviours to generate insights and provide commercial recommendations with Data Wrangling, Validation, Visualization in Python.

* Performed Experimentation, uplift testing & commercial application with Data analysis, Statistical testing, reports building,etc

## Dataset:
The datasets are taken from client and data has following features:
### Transaction (size_264836 rows × 8 columns):
*	DATE 
*	STORE_NBR 
*	LYLTY_CARD_NBR 
*	TXN_ID 
*	PROD_NBR
*	PROD_NAME
*	PROD_QTY 
*	TOT_SALES

### Behaviours (size_72637 rows × 3 columns):
*	LYLTY_CARD_NBR 
*	LIFESTAGE
*	PREMIUM_CUSTOMER



## Data Cleaning
After collecting the data, I needed to clean it up so that it was usable for further processing. I made the following changes and created the following variables:

* Converted date string data type to datetime datatype 
* Extracted first name from product name as the brand name
* Extracted the last word from product namewhich is the pkg details
* Extracted only numeric characters as weight term
* Filled missing or null values with mode value
*	Dropping unnecessary ID column from dataset
*	Removed duplicate rows
*	Merged two tables on a common column
*	And made many more changes which can be viewed in the pre-processed data in csv file


## Exploratory Data Analysis (EDA)
Performed EDA on the cleaned data and got various insights, relationships, etc, few of them are as below.
![image](https://user-images.githubusercontent.com/112246352/198828788-ab2ebac1-c6f8-4df4-98b2-138d291b52ac.png)

![image](https://user-images.githubusercontent.com/112246352/198828801-f867aee8-1fd6-4d23-9da1-6c12c5135612.png)


![image](https://user-images.githubusercontent.com/112246352/198828807-2ad0afb4-bc9b-423e-9a34-14af3fe81d3f.png)

## Model Building 

First, I transformed the categorical variables into dummy variables, then scaled with standard scaler from sk-learn. I also split the data into train and tests sets with a test size of 20%.   

I tried Logistic Regression model and evaluated using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren’t particularly bad in for this type of model.   

I tried three different models:
*	**Logistic Regression** – for prediction of categorical outcomes, with the sparsity associated with the data, I thought that this would be a good fit.  

## Model performance
The Logistic Regression model far outperformed the other approaches on the test and validation sets. 
*	**Logistic Regression** : MAE = 24%



## Productionization 
In this step, I saved the prepared model using pickle module for further deploymnet. Then Created a absenteeism_module for deployment.Finally, Analyzed the Predicted Outputs in Tableau for various variables.



## Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, sklearn, pickle

**The Data Science Course 2022: Complete Data Science Bootcamp**
https://www.udemy.com/course/the-data-science-course-complete-data-science-bootcamp/

**Ken Jee Youtube channel**
https://www.youtube.com/c/KenJee1







