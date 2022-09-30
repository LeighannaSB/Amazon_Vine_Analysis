# Amazon Vine Analysis

![image](https://user-images.githubusercontent.com/107161421/193179785-2625a8ea-250a-4988-98d5-0b948a6c8667.png)

## Overview

The purpose of this analysis was to compare the ratings for all items in Amazon's "outdoor" category for any potential bias in the reviews left by members of their Vine program. The two deliverables for this analysis were:

- Perform ETL on Amazon Product Reviews
- Determine Bias of Vine Reviews

The outdoor products data was pulled from an AWS RDS database into pgAdmin to create the necessary tables from the data and into Google Colab to clean up the data and create dataframes from the data. 

Creating dataframes in Colab

![image](https://user-images.githubusercontent.com/107161421/193178871-b8d90bf3-ea1c-485e-a594-60cbc29fd0e0.png)


Creating tables in pgAdmin (Customers, Products, Reviews, Vine)

![image](https://user-images.githubusercontent.com/107161421/193178969-1bfe13af-fd24-423e-a9de-bdd9a24109fc.png)
![image](https://user-images.githubusercontent.com/107161421/193179038-d97e2463-53e1-498f-8089-ac294b73aae4.png)
![image](https://user-images.githubusercontent.com/107161421/193179088-dd5ed206-782b-4f47-b29c-14e5373da0c5.png)
![image](https://user-images.githubusercontent.com/107161421/193179141-893a7634-d895-422b-a75b-c5871eedfca3.png)


## Results

After cleaning and analyzing the data the following was found:

- There were 107 total Vine (paid) reviews and 39869 total unpaid review

![image](https://user-images.githubusercontent.com/107161421/193177326-11bccb54-4cc1-4eeb-bee3-f2958ef29136.png)
![image](https://user-images.githubusercontent.com/107161421/193177358-cf919f66-8bfe-44eb-8b8e-937628822304.png)

-There were 56 five star reviews left by Vine (paid) members and 21005 five star reviews left by unpaid users

![image](https://user-images.githubusercontent.com/107161421/193177533-07e775e3-9db4-4fb7-950a-accf3da69307.png)
![image](https://user-images.githubusercontent.com/107161421/193177575-28b0bc06-6803-47e8-9e02-cd69e297c281.png)

- The total percentage 0f five star Vine (paid) reviews was 52.34% and the total percentage of five star unpaid reviews was 52.69%

![image](https://user-images.githubusercontent.com/107161421/193177818-11657bd8-89cb-4c45-a4bc-05628fc2d5a5.png)
![image](https://user-images.githubusercontent.com/107161421/193177846-cb91136b-d241-4e8e-b972-2f3970c4a973.png)

## Summary

The analysis did not find any positivity bias for reviews in the Vine program, in fact the unpaid reviews were ever so slightly more likely to be positive. This difference was less than a full percentage. Further analysis could be done on different product categories to confirm this is the case site wide and not isolated to the outdoor equipment. Analyzing further product categories could also be beneficial as there were only 107 paid reviews compared to the nearly 40000 unpaid reviews. 
