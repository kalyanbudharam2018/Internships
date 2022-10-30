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




## Analytics and commercial application
 
In this task, I saved the prepared files for further application. From previous tasks, I prepared a report for the client and the Category Manager. Report mainly consists of following details:
### Chips Category Review
● Chips transactions increase substantially prior to Christmas. It is a good time totake advantage of this momentum with promotional offers.
● Older and Young Family segment have the highest average purchase units per
unique customer.
● Sales mainly came from Budget - older families, Mainstream - young
singles/couples, and Mainstream -retirees. In total contributing 25% of sales
revenue.

### Trial Store Analysis
● Trial store 77 and 86 experienced significant increase in Total Sales and
Customers quantity during the trial period compared to their control stores..
● Trial store 88 experience increase as well, but insignificant compared to
its’ Control store.




## Code and Resources Used 
**Python Version:** 3.7  
**Packages:** pandas, numpy, seaborn, matplotlib

**Quantium_Forage website**
https://www.theforage.com/virtual-internships/NkaC7knWtjSbi6aYv?ref=GoP4G9dwRbsQ3n9PB







