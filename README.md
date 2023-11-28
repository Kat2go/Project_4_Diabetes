# Project_4_Diabetes
## Table of Contents
* [About](#about)
* [Tools](#tools)
* [Analysis](#analysis)
* [Results](#results)
* [Summary](#summary)
## About
In the final project of Group 2's project for the DU Data Analytics and Visualization Boot Camp, team members Katrina Brown, Triston Cavaness, Lesley Conn and Juliet Hamilton accessed data from Kaggle and the U.S. Centers for Disease Control (CDC)  to determine the extent of correlation of diagnosis of Type 2 diabetes onset in male and female populations based on factors of age, body mass index (an obesity indicator), smoking history, hypertension,fasting and non-fasting blood glucose levels, and heart disease. Kaggle data contained 100,000 rows of data; CDC information provided 2018 research on diabetes and obseity for more than 3,000 counties in the United States. One limitation of data in both sources was patient race and/orethnicity, though some hypothesis were developed after mapping the CDC data bsed on county codes, then referencing locations against U.S. Census data for those counties.
## Tools
* Python
* PANDAS
* pathlib
* pyspark
* sklearn.metrics
* Tableau
## Analysis
The Kaggle data was imported, reviewed for nonnulls and data types and an initial histogram view of each data type was developed to document distribution of data by gender and health condition. After the data cleanup, the updated dataframe was split into the target and feature variables, followed by a train-test split. A logistic regression model was applied to the test portion, resulting in predictions. Evaluation metrics, including balanced accuracy score, confusion matrix, and classification report, were computed to assess the model's performance. (MORE HERE)
Before CDC data could be imported into Tableau, 

**Logistic Regression on Training Data:**  
* Balanced accuracy score: %  
* Precision: %  
* Recall: %  

## Results
Diabetes and health factors -- strong relationship between the Type 2 disease and hypertension, high blood sugar but not as strong a causal relationship between overweight and diabetes.
CDC geographic data -- highest percentages of diabetes and obesity combined is in Kentucky/West Virginia Appalachian region but similar spike in "high/high" bivariate choropleth were also revealed in South Dakota, in the South, particularly in rural South Carolina and along Gulf Coast regions. 

## Summary
  
