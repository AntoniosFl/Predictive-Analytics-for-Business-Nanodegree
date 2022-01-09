# The Business Problem #
You recently started working for a company that manufactures and sells high-end home goods. Last year the company sent out its first print catalog, and is preparing to send out this year's catalog in the coming months. The company has 250 new customers from their mailing list that they want to send the catalog to.

Your manager has been asked to determine how much profit the company can expect from sending a catalog to these customers. You, the business analyst, are assigned to help your manager run the numbers. While fairly knowledgeable about data analysis, your manager is not very familiar with predictive models.

You’ve been asked to predict the expected profit from these 250 new customers. Management does not want to send the catalog out to these new customers unless the expected profit contribution exceeds $10,000.

# Details #
  * The costs of printing and distributing is $6.50 per catalog.
  * The average gross margin (price - cost) on all products sold through the catalog is 50%.
  * Make sure to multiply your revenue by the gross margin first before you subtract out the $6.50 cost when calculating your profit.

Write a short report with your recommendations outlining your reasons why the company should go with your recommendations to your manager.

## Project Walkthrough ##

### Step 1: Business and Data Understanding ###
The project includes a description of the key business decisions that needed to be made.

### Step 2: Analysis, Modeling, and Validation ###
I Built a linear regression model, which I then used to predict sales for the 250 customers. I used Alteryx for the linear model build.

The prediction for the sales for the individual people in the mailing list have been calculated with the linear regression equation from the linear regression model

### Step 3: Writeup ###
Lastly I created a report with my recommendation.

## Data ##

[*p1-customers.xlsx*](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/predicting-catalog-demand/p1-customers.xlsx) - This dataset includes the following information on about 2,300 customers.

[*p1-mailinglist.xlsx*](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/predicting-catalog-demand/p1-mailinglist.xlsx) - This dataset is the 250 customers needed to predict sales. This is the list of customers that the company would send a catalog to. This dataset was used to estimate how much revenue the company can expect if they send out the catalog. It includes all of the fields from P1_Customers.xlsx except for `Responded_to_Last_Catalog` **so this variable was not used in the linear regression model since it could not be applied to the mailing list data set.** It also includes two additional variables.

  * Score_No: The probability that the customer WILL NOT respond to the catalog and not make a purchase.
  * Score_Yes: The probability that the customer WILL respond to the catalog and make a purchase.
