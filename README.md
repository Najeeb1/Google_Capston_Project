# Google Data Analytics Capstone Project: Bike-Share
### Quick Links:

[Preporcessing with Pandas](https://github.com/Najeeb1/Google_Capston_Project/blob/main/process.ipynb)

[Analysis with R](https://a1104c4c2c6842deb059c153deafd12e.app.posit.cloud/file_show?path=%2Fcloud%2Fproject%2FBike_Rideship_Analysis.html)

[Visualization with Tableau](https://public.tableau.com/app/profile/najeebullah.hussaini/viz/BikeRidershipAnalysisQ19Q20/Bike_Ridership_Analysis)


## Contents
- [Introduction](#Introduction)
- [Ask](#Ask)
- [Prepare](#Prepare)
- [Process](#Process)
- [Analyze and Share](#Analayze-and-Share)
- [Act](#Act)
- 

## Introduction: 
In this case study, I will perform many real-world tasks as a data analyst. To answer the key business questions, I will follow the steps of the data analysis process: Ask, Prepare, Process, Analyze, Share, and Act.

The course can be accessed: [Google Data Analytics Capstone: Complete a Case Study](https://www.coursera.org/learn/google-data-analytics-capstone)


The dataset can be accessed: [divvy_tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html) 

#### Background: 
Cyclistic: A bike-share program features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8% of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use bikes to commute to work each day.

#### problem statement: 
You are a junior data analyst on the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.

## Ask
Three questions will guide the future marketing program: 

1. How do annual members and casual riders use Cyclistic bikes?
2. Whywouldcasualriders buy Cyclistic annual memberships?
3. HowcanCyclistic use digital media to influence casual riders to become members? Moreno has assigned you the question to answer: How do annual members use Cyclistic bikes differently?

## Prepare: 

I have worked with two different types of datasets. a) quarterly ridership of 2019 and 2020. b) all 12 months of 2023. 
Every analysis and visualization belongs to the first dataset. Only the Preprocess file done with Python belongs to the second one. 
The reason for the later part was to be able to work with complex SQL queries. However, Google BigQuery limit exceeds very fast. 
I picked Pandas to do it for free. 

## Process: 
In the processing part, I have done mostly cleaning and combining datasets and having an overview of the data. Feel free to check them here: 
[Preporcessing with Pandas](https://github.com/Najeeb1/Google_Capston_Project/blob/main/process.ipynb) and 
[Analysis with R](https://a1104c4c2c6842deb059c153deafd12e.app.posit.cloud/file_show?path=%2Fcloud%2Fproject%2FBike_Rideship_Analysis.html)

## Analayze and Share
I started with the analysis of a single month's data. This is useful as it is easy to work with, takes less time to get a quick pick, and builds some understanding of the data. 
Additionally, the dataset size is small and is manageable by using Google Sheet or Excel both of which have handy features such as pivots and filters. Let us take a look at the average ride duration for each user type for each day of the week from January 2023. 

The X-axis shows the type of users and the Y-axis shows the time minutes. 
![Average ride duration for each user type every weekday](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/chart1.png)

We know that casual users ride duration is longer. However, when it comes to the total number of rides, it is completely the opposite. 

The X-axis shows the type of users and the Y-axis shows the total number of rides. 
![Total number of rides for each user type every weekday](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/chart3.png)


Now let us take a look at the monthly ridership average and total: 

![Average ride duration for each user type every month](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/mavg.png)

One observation that can be made here is the fact that during summer on average casual riders spike. This can be attributed to warm weather and summer vacations. 

![Total number of rides for each user type every month](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/mtotal.png)

We can also take a look at the weekly average and total for each user type. 

![Average ride duration for each user type every week](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/wavg.png)

Here we can see that during the weekends the casual users ride more than usual. This indicates again that casual users take rides for leisure activities and free days of the week. 

![Total number of rides for each user type every week](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/wtotal.png)

Now let us see the hourly changes. 

![Average ride duration for each user type every hour](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/havg.png)

Here we can see that member users plan their rides while the hourly ride for casual users seem to be very chaotic and can change frequency fast. 

![Total number of rides for each user type every hour](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/htotal.png)

Finally, let us take a look at the top destinations for each user type. 

![Top destinations for member users](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/mdest.png)

We can see that member users usually go to universities and businesses.  
And top destination for casual users: 

![Top destinations for casual users](https://github.com/Najeeb1/Google_Capston_Project/blob/main/images/cdest.png)

Here, the casual users prefer to go to Parks, Museums, Theaters and sightseeing. 

## Act


