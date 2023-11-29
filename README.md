# Project_4_Diabetes
## Table of Contents
* [About](#about)
* [Tools](#tools)
* [Analysis](#analysis)
* [Results](#results)
* [Summary](#summary)
## About
In the final Group 2 project for the June 2023 DU Data Analytics and Visualization Boot Camp, team members Katrina Brown, Triston Cavaness, Lesley Conn and Juliet Hamilton accessed data from Kaggle and the U.S. Centers for Disease Control (CDC) to determine the extent of correlation between diagnosis of Type 2 diabetes onset in male and female populations and the factors of age, body mass index (an obesity indicator), smoking history, hypertension,fasting and non-fasting blood glucose levels, and heart disease. Kaggle data contained 100,000 rows of data; CDC information provided 2018 research on diabetes and obseity for more than 3,000 counties in the United States. One limitation of data in both sources was patient race and/orethnicity, though some hypotheses were developed after mapping the CDC data bsed on county codes, then referencing locations against U.S. Census data for those counties.
## Tools
* Python
* PANDAS
* pathlib
* pyspark
* sklearn.metrics
* Tableau
## Analysis
The Kaggle data was imported, reviewed for nonnulls and data types and an initial histogram view of each data type was developed to document distribution of data by gender and health condition. After the cleanup, the updated data was split into the target and feature variables, followed by a train-test split using sci-kit learn's metric and standard scaling. A logistic regression model was applied to the test portion, resulting in two predictions. Evaluation metrics, including balanced accuracy score, confusion matrix, and classification report, were computed to assess the model's performance.
The first model attained an accuracy score of 95.82% and F1 scores of 98% (Class 0 for detecting no diabetes) and 72% (Class 1 for detecting diabetes) on the harmonic of precision and recall. The noticeable difference in the precision and recall for Class 1 indicates that the model struggled more with correctly identifying instances of diabetes. The second model, employing imblearn.over_sampling, achieved a lower accuracy of 88.55% and F1 scores of 93% (Class 0 for detecting no diabetes) and 57% (Class 1 for detecting diabetes). Examination of the recall scores (a subcomponent of the F1 scores for model predictability accuracy) shows more consistent scoring across the four classes while precision in Class 1 from Model 1 to Model 2 dropped by 50%. That lack of precision, along wtih a greater imbalance across the two classes, results in a lower accuracy for the second model.
Before CDC data could be imported into Tableau, FIPS codes for each county had to be uniformly formatted into a 5-digit code. Additional research was required to ascertain the definitions within the CDC choropleth legend for HH, HM, HL, MH, MM, ML, LH, LM, LL. The acronyms denote combined findings within each U.S. county for high, medium, and low rankings for the often-related conditions of obesity and Type 2 diabetes.

## Results
Diabetes and health factors -- strong relationship between the Type 2 disease and hypertension, high blood sugar but not as strong a causal relationship between overweight and diabetes.
CDC geographic data -- highest percentages of diabetes and obesity combined is in Kentucky/West Virginia Appalachian region but similar spike in "high/high" bivariate choropleth were also revealed in South Dakota, in the South, particularly in rural South Carolina and along Gulf Coast regions. 

## Summary
  
