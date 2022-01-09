# Project Overview #
You are a loan officer at a young and small bank (been in operations for two years) that needs to come up with an efficient solution to classify new customers on whether they can be approved for a loan or not. You'll use a series of classification models to figure out the best model and provide a list of creditworthy customers to your manager.

## The Business Problem ##

You work for a small bank and are responsible for determining if customers are creditworthy to give a loan to. Your team typically gets 200 loan applications per week and approves them by hand.

Due to a financial scandal that hit a competitive bank last week, you suddenly have an influx of new people applying for loans for your bank instead of the other bank in your city. All of a sudden you have nearly 500 loan applications to process this week!

Your manager sees this new influx as a great opportunity and wants you to figure out how to process all of these loan applications within one week.

Fortunately for you, you just completed a course in classification modeling and know how to systematically evaluate the creditworthiness of these new loan applicants.

For this project, you will analyze the business problem using the Problem Solving Framework and provide a list of creditworthy customers to your manager in the next two days.

You have the following information to work with:

  1. Data on all past applications
  2. The list of customers that need to be processed in the next few days

## Project Walkthrough ##

### Step 1: Business and Data Understanding ###
The project includes a description of the key business decisions that need to be made.

### Step 2: Exploration and Cleanup of the Data ### 
The exploration and cleanup of the data included:

  1. Check of data fields with high correlation (correlation > .70).
  2. Check for missing data for each of the data fields.
  3. Check for data fields with "low variability”.

## Step 3. Classification Models training ## 
Training set was 70% and Validation set 30%.

The dataset was trained using the following models:

  * Logistic Regression
  * Decision Tree
  * Forest Model
  * Boosted Tree

## Step 4. Writeup ##
The models’ performance were compared against each other. New customers were scored based on the best model.

A brief report on how I came up with the classification model was written as well as the number of new customers who would qualify for a loan.


### Data ###

[*credit-data-training.xlsx*](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/predicting-default-risk/credit-data-training.xlsx) - This file contains all credit approvals from your past loan applicants the bank has ever completed.

[*customers-to-score.xlsx*](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/predicting-default-risk/customers-to-score.xlsx) - This is the new set of customers that were scored on the classification model I built.
