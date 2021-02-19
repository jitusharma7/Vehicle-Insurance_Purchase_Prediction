# Vehicle-Insurance_Purchase_Prediction
The aim of this project  is to predict whether the customer will be interested in purchasing additional insurance for vehicles


## Table of Content
  * [Overview](#Overview)
  * [Dataset](#Dataset)
  * [Approach](#Approach)
  * [Result](#Result)
  

## Overview
Building systems for customer segmentation which ease in targeting potential customers for selling products or services is a huge requirement in companies these days. The use may be of insurance, user subscription and many more.

One of major problem aligh with above mentioned problem regarding customer segmentation that whether customer will buy insurance or not.We'll use a logistic regression classifier and build model.We also use ROCR Curve for getting  threshold value and check accracy for the model.


## Dataset
The dataset consists of the following attributes:

* id (Unique ID for the customer)
* Gender
* Age
* Driving License (0: Not present, 1: have one)
* Region_Code
* Previously_Insured (1: already has insurance, 0: doesn't have)
* Vehicle_Age
* Vehicle_Damage (1: customer got vehicle damage in past, 0: no past history of damage)
* Annual_Premium (Amount to be paid annually)
* PolicySalesChannel
* Vintage (Number of days customer has been in the company)
* Response ('Target Column' ) (1: Customer is interested, 0: not interested)


## Approach

The approach for this project is expaline with following steps - 
1. Step1     __Understanding Dataset with business problem perspective__
   - What is importance of each attributes and what would be impact on insurance buying decison.
    




<img src="/vehicle%20damage%20vs%20target%20variable.png" width="300">
