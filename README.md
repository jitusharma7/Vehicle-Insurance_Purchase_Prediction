# Vehicle_Insurance_Purchase_Prediction
This project aims to predict whether the customer will be interested in purchasing additional insurance for vehicles.

## Table of Content
  * [Overview](#Overview)
  * [Dataset](#Dataset)
  * [Approach](#Approach)
  * [Result](#Result)
  * [Credit](#Credit)
  

## Overview
Building systems for customer segmentation which ease in targeting potential customers for selling products or services is a huge requirement in companies these days. The usage may be insurance, user subscription, and many more.

One of the major problems aligns with the above-mentioned problem regarding customer segmentation that whether the customer will buy insurance or not. We'll use a logistic regression classifier and build the model. We also use ROCR Curve for getting threshold values and check accuracy for the model.

## Dataset
The dataset consists of the following attributes:

* id (Unique ID for the customer)
* Gender
* Age
* Driving License (0: Not present, 1: have one)
* Region_Code
* Previously_Insured (1: already has insurance, 0: doesn't have)
* Vehicle_Age
* Vehicle_Damage (1: customer got vehicle damage in past, 0: no history of damage)
* Annual_Premium (Amount to be paid annually)
* PolicySalesChannel
* Vintage (Number of days customer has been in the company)
* Response ('Target Column' ) (1: Customer is interested, 0: not interested)


## Approach

The approach for this project is explained with the following steps - 
1. ***Step1***     __Understanding Dataset with business problem perspective__
  - What is the importance of each attribute and what would impact on insurance buying decision due to various feature 

2.  ***Step2***     __Data Preprocessing__
  2.  ***Step2***     __Data Preprocessing__
   - check NA value in each feature 
   - drop ID feature due to high cardinality
   - Apply one-hot encoding to rest of categorical feature using drop_first argument to avoid extra column created during one-hot encoding
   - use heatmap for correlation 
 
 
<img src="/Correlation%20HeatMap.png" width="300">
   -  use bar chart - Gender vs vehicle damage impact
  
<img src="/vehicle%20damage%20vs%20target%20variable.png" width="300">

3. ***Step3***     __Model Building__
  3. ***Step3***     __Model Building__
   - LogisticRegression - Machine learning technique used for this classification problem
   - Split the dataset into training and testing dataset
   - performance in terms of predicting false negative values is crucial because it is important to know who will buy the insurance.
   - F-score of the model is highest when using the weighted method
   - using ROCR Curve  it shows that - threshold probability value = 0..65

   
  <img src="ROCR%20Curve.png" width = "350">
  
  
  
  ## Result
  - Model Accuracy - 0.87
  - Vehicle damage and Age are the important features to drive the decision whether to buy vehicle insurance or not
  - 5% of the total observations - false negative value.

  ## Credit

 - [dockship](https://https://dockship.io/) - This project has been done on this competitive platform.

