---
layout: post
title: Diabetes Dataset Project
tags: Statistical Inferences
---

#Introduction
I chose this data set because my wife has diabetes.  Originally, I wanted to see what variables would predict the occurrance of diabetes, but I have learned that. I found my dataset at Kaggle and it was collected by National Institute of Diabetes and Digestive and Kidney Diseases.  I am sure that there is a relationship between age, Body Mass Index(BMI) and a positive or negative result for diabetes.  I decided the best approach would be to use a Chi-square hypothesis test to determine if there was any relationship between these variables.

#Description of the Data
I found my data on the website Kaggle. It was collected by the National Institute of Diabetes and Digestive and Kidney Diseases in order to see what variables would predict someone getting type 2 diabetes. It contains variables BMI, age, skin thickness, blood pressure and number of pregnancies. This set is limited to all females, age 21 and older and Pima Indian heritage. There is no information on diet, exercise, or genetics which are all predictors for diabetes as well.

#Statistical Methods
My hypothesis is that there is a relationship between BMI and age, and whether a person has type 2 diabetes. I will isolate both BMI and age to compare them with a positive of negative result.
I looked up what BMI threshold was reached to be considered obese and that result was greater than or equal to 25. I took the column that was BMI in my set and engineered it to be normal for anyone with a BMI under 25 and overweight for those equal to or above and named this column BMI_Adj. I engineered the age column to select women that were younger than 50 to be 50 - 90 and the rest went into 21 - 49. This column I renamed Age_Cat. I used the Chi-squared statistical test since the data is descrete and compared the p-values of each to see if they were statitically significantly related with 5% variance.

#Results
Using the Chi-squared test, I was able to demonstrate that there is an association between BMI and diabetes with a p-value of 4.11 x 10^-11 compared to an alpha threshold of 0.05 it is less. I was also able to show that age is also associated with diabetes as well with a p-val of 0.0068 also less than 0.05.

#Conclusion
I conclude that from this analysis, using data taken from 21 year-old females of the Pima Indians, that there is a statistically significant association between BMI and diabetes and age and diabetes. This study is important because many individuals are in jeopardy of developing type 2 diabetes. Any predictive study will help individuals make better health decisions about their lives and decrease the numbers of people obtaining it. According to the Centers for Disease Control and Prevention(CDC), 1 in 10 adults have diabetes. The CDC has also seen a decrease in the numbers of people over 20 years old but there is much room for improvement. The dataset I used is limited to a specific population, sex and age of people. It lacks information about diet, exercise and genetics, all of which are valid variables to check for in predicting someone getting diabetes. In the same study done by the CDC, they also have shown that there is a link between BMI and people having diabetes. Of the people having diabetes 89% are overweight CDC data. My hope for this research was to use new data science techniques from Python and its associated libraries to make statistical inferences from a data set. I was able to prove my hypothesis was statistically significant for an association between BMI ~ diabetes and age ~ diabetes.
