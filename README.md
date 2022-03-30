This repository contains the files for the Group Project task of Group 5 for COMP2200/6200 in S2 2021.

# Analysis on House Rent and Sales in NSW, Australia

## Group Members:
- Aarushi Chaudhary - 46113908
- Ameer Ali Mavani - 46812342
- Arnav Bajaj- 46806423
- Kaveri Bhatia Chanana - 46282920

## Introduction

The property market in New South Wales, particularly in Sydney, has been rising in recent years. The cost has increased by nearly 15% in the last year. As the number of individuals coming to NSW to study or work increases, everyone should be able to find a sustainable and suitable home to live that is both affordable and safe. We will utilize data on income, crime, housing sales and rent to characterize all of NSW’s Local Government Areas (LGAs) and see if there is a relationship between them.

## Problem Statement and Goals

Our main 3 goals in this Analysis project are:

- To predict the number of house sales for all LGA's based on the crime rate and income data.
- Clustering LGAs based on Rent, Sales, crime and Income etc.
- Classification model based on rent, sales, crime and income data.

## Data and Files

We planned our work to all be done on the same notebook now titled "Final Report Analysis.ipynb" by communicating with each other effectively and having weekly meetings.

Our data files are sourced from the links given below:

Rent and Sales data - [NSW Department of Family and Community Service](https://www.facs.nsw.gov.au/resources/statistics/rent-and-sales/dashboard)

Income Data - [Australian Bureau of Statistics Census](https://www.abs.gov.au/statistics/labour/earnings-and-work-hours/personal-income-australia/latest-release#data-download)

Crime Data - [NSW Bureau of Crime Statistics and Research](https://www.bocsar.nsw.gov.au/)

## Some Data Exploration

![image](https://user-images.githubusercontent.com/87954953/140260782-48625886-9df6-44dd-b89a-645881b6efa7.png)


The above bar graph, represents the average rent for all LGA's in the 2nd quarter(July 2021). The yellow line represents the average rental mean, which represents the average of all LGA's which is $186.27. And the highest rental cost is in Sydney.

![image](https://user-images.githubusercontent.com/87954953/140260826-4af32260-f8b0-4fea-8954-cea865bf0567.png)

From the above graph, we can infer that Ku-Ring-Gai has the highest house prices at almost 2 Million AUD followed by Hunter's Hill, Woolahara and Mossman. The Average house price is around $600,000

![image](https://user-images.githubusercontent.com/87954953/140260857-75b5e23e-6adf-4488-9a70-fa33f7be53be.png)

From the above graph, it is evident that maximum total no of crimes are committed in Blacktown LGA.

![image](https://user-images.githubusercontent.com/87954953/140260965-d9137086-60cd-4782-8650-f7371f0e12ac.png)

We see the area with the highest income are Woollahara and North Sydney at over $70,000 Median income. The Average across NSW is around 48,000 AUD.

## Conclusion and Future Improvements

In line with our goals for this project we were able to fit a Linear Regression model to predict the number of sales in any LGA in New South Wales based on the Median income and total number of crimes. We found that number of earners has a high positive correlation with the number of sales. As there are more earners, the earnings in each household also increases. This enables them to invest their money to buy properties and hence we see an increase in number of house sales.

Using the KMeans clustering alogrithm, we see 3 distinct clusters to divide the various LGA's distinguishable based on Income, House Sales price, Weekly Rent and Number of sales.These clusters could be labeled as "Lower Middle Class", "Upper Middle Class" and "Rich Class". One unique feature we noticed is the number of crimes in the 'Upper Middle Class' region is the highest and the 'Rich Class' area it is the 2nd highest. This could be due to the better security features in the 'Rich Class' area.

Based on this clustering we then created a K-Nearest Neighbour model to classify the regions. We split our data into train and test and created a model with an accuracy score of 0.92. This model hopefully could classify LGA's in other regions.

While the models we created do seem to have a high accuracy, it is possible this is due to a slight overfitting issue as our datasize is small. There could be various other factors that could be affecting the output we wished to achieve.

Moving forward we would build on this project by adding more features affecting the Sales and Rent in different LGA and by using data from all the years that it is avalaible.
