# Capstone Project Overview #
The capstone project has three main tasks, each of which requires you to use skills you developed during the Nanodegree program. Once you complete all three tasks, please submit the project as a PDF.

- ## **Task 1: Store Format for Existing Stores** ##

  Your company currently has 85 grocery stores and is planning to open 10 new stores at the beginning of the year. Currently, all stores use the same store format for selling their products. Up until now, the company has treated all stores similarly, shipping the same amount of product to each store. This is beginning to cause problems as stores are suffering from product surpluses in some product categories and shortages in others. You've been asked to provide analytical support to make decisions about store formats and inventory planning.
  
  ![alt text](https://video.udacity-data.com/topher/2019/August/5d47a326_man-climbing-up-in-grocery-store-115680/man-climbing-up-in-grocery-store-115680.jpg)

- ### **Determining Store Format** ###
To remedy the product surplus and shortages, the company wants to introduce different store formats. Each store format will have a different product selection in order to better match local demand. The actual building sizes will not change, just the product selection and internal layouts. The terms "formats" and "segments" will be used interchangeably throughout this project. The goals of this part were:
  
   * To determine the optimal number of store formats based on sales data.

      This was achieved by:
      * Summing sales data by StoreID and Year
      * Using percentage sales per category per store for clustering (category sales as a percentage of total store sales).
      * Using only 2015 sales data. 
      * Using a K-means clustering model.

   * To segment the 85 current stores into the different store formats.

Data that was used:
  * [*StoreSalesData.csv*](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/combining-predictive-techniques/storesalesdata.csv) and 
  * [*StoreInformation.csv*](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/combining-predictive-techniques/storeinformation.csv) files.
   
- ## **Task 2: Store Format for New Stores** ##

  The grocery store chain has 10 new stores opening up at the beginning of the year. The company wants to determine which store format each of the new stores should have. However, we don’t have sales data for these new stores yet, so we’ll have to determine the format using each of the new store’s demographic data.
  
  ![alt text](https://video.udacity-data.com/topher/2019/August/5d47a544_construction-in-toronto-may-2012/construction-in-toronto-may-2012.jpg)

- ### **Determine the Store Format for New Stores** ###
Goals:

  * To develop a model that predicts which segment a store falls into based on the demographic and socioeconomic characteristics of the population that resides in the area around each new store.
  * To use a 20% validation sample with Random Seed = 3 when creating samples with which to compare the accuracy of the models. 
  * To compare a decision tree, forest, and boosted model.
  * To use the model to predict the best store format for each of the 10 new stores.
  * To use the [StoreDemographicData.csv](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/combining-predictive-techniques/storedemographicdata.csv) file, which contains the information for the area around each store.

  - ## **Task 3: Forecasting** ##

  Fresh produce has a short life span, and due to increasing costs, the company wants to have an accurate monthly sales forecast.
  
  ![alt text](https://video.udacity-data.com/topher/2019/August/5d479d48_22219503122-065a9f04be-b/22219503122-065a9f04be-b.jpg)

- ### **Forecasting Produce Sales** ###
  Goals:
  
 * To prepare a monthly forecast for produce sales for the full year of 2016 for both existing and new stores using a 6 month holdout sample for the TS Compare tool as we do not have that much data and using a 12 month holdout would remove too much of the data.

 * To forecast produce sales for existing stores I aggregated produce sales across all stores by month and created a forecast.

 * To forecast produce sales for new stores. To do so:
    * I Forecasted **produce sales (not total sales)** for the average store (rather than the aggregate) for each segment.
    * Multiplied the average store produce sales forecast by the number of new stores in that segment.
    * Summed the new stores produce sales forecasts for each of the segments to get the forecast for all new stores.

 * To Sum the forecasts of the existing and new stores together for the total produce sales forecast.
   


### **Data** ###

  * [StoreSalesData.csv](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/combining-predictive-techniques/storesalesdata.csv) - This file contains sales by product category for all existing stores for 2012, 2013, and 2014.
  * [StoreInformation.csv](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/combining-predictive-techniques/storeinformation.csv) - This file contains location data for each of the stores.
  * [StoreDemographicData.csv](https://github.com/AntoniosFl/Predictive-Analytics-for-Business-Nanodegree/blob/main/combining-predictive-techniques/storedemographicdata.csv) - This file contains demographic data for the areas surrounding each of the existing stores and locations for new stores.




