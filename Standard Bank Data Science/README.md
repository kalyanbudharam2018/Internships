
# Prediction of Loan application status: Project Overview 

* Business Problem: Currently the home loan application process is a manual one. It which takes 2-3 days, which mean that the applicant will only be notified after 2-3 days of the application outcome.

* Business Objective: Reduce the amount of time it takes for applicants to be notified about their loan statuses (to a matter of seconds).

* Hypothesis: Based on historical data we can use machine learning to predict the loan status of a potential borrower such that the time taken for them to receive their respective statuses is reduced significantly.


* Created a tool that predicts the loan status of a potential borrower which will helpful to the bank as well as applicants such that the applicant receives a response immediately after completing their application.


## Summary:
*	Worked for 'Loan Prediction’ business problem on historical bank data (dataset@ Client_size-981, 13) by implementing Data pre-processing & Exploratory Data Analysis (EDA with Sweetviz) using SQL, Python & libraries.
*	Machine Learning Production with AutoML (79%) & Random Forest Classifier (77%) using Scikit-Learn.
*	Prepared to present the insights to a non-technical audience through communication.


## Dataset:
This dataset is taken from Kaggle which is famous for it employment service and data has following features:
*	Loan_ID
*	Gender             
*	Married            
*	Dependents         
*	Education           
*	Self_Employed      
*	ApplicantIncome    
*	CoapplicantIncome  
*	LoanAmount         
*	Loan_Amount_Term    
*	Credit_History     
*	Property_Area      
*	Loan_Status        



## Data Cleaning
After collecting the data, I needed to clean it up so that it was usable for our model. I made the following changes and created the following variables:

*	Dropped unnecessary Loan_ID column from dataset
*	Did some one hot encoding for categorical columns
*	Reordered the columns like original dataset order
*	Updated the null values with their mean, mode values and some deleted
*	And made many more changes which can be viewed in the pre-processed data csv

## Exploratory Data Analysis (EDA)
Performed EDA on the cleaned data and got various insights, relationships, etc, few of them are as below.

* Loan status details are as follows.
  Y    68.7296%
  N    31.2704%
  
Gender  Loan_Status    %
Female  Y              66.9643
        N              33.0357
Male    Y              69.3252
        N              30.6748
        
![download](https://user-images.githubusercontent.com/112246352/203770363-fdac9810-83a0-4864-82f0-dc29f771836f.png)


![download](https://user-images.githubusercontent.com/112246352/203770528-ae63b975-b17a-4f81-b6fc-1769fbf392be.png)


## Model Building 

First, I transformed the categorical variables into dummy variables, then scaled with standard scaler from sk-learn and the datasets are already splits into train and test sets.   

I tried different Machine Learning models:
*	** Auto ML wth autosklearn** – for prediction of categorical outcomes and no need much pre-processing.
*	** Random Forest Classifier **  - for prediction of categorical outcomes, with the sparsity associated with the data and for easy interpretation. 


## Model performance
The models performed good on the test and validation sets and the results are as given below. 
	                   **AutoML**     **Random Forest Classifier**
**Accuracy**           79%            77%




## Productionization 
In this step, I saved the prepared model using pickle module for further deploymnet and application. 


## Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, auto-sklearn, sklearn, pickle

**Standard_Bank_Forage website** 
https://www.theforage.com/virtual-internships/






