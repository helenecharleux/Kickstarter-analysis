# An analysis of Kickstarter campaigns
Our client, Louise, would like to suppport the creation of the play "Fever". She would like to start a crowdfunding campaign. Whith a total budget of $10,000, she is looking for recommandations to make a success with her first fundraising campaign. She wants to understand whether there are factors to make fundraising campaigns successful. 
We purpose Louise to work on our Kickstarter database in order to plan a successful campaign to support her project.
## 1. Presentation of the database and challenges
Our database Kickstarter is a large database of 4.113 projects.
![Screenshot database](https://user-images.githubusercontent.com/85641189/122977759-64b4fe80-d35b-11eb-8a9d-cea4d4d60447.png)
 With a total of 12 variables, we are able to highlight trends on the Theater category and for the US market. However we  have to change some variables for the dataset to be readable and to answer Louise's concerns.
 ### 1.1 Changing the Deadline and Launched_at columns into readable data 
 The Deadline and Launched_at columns coutain Unix timestamps rather than dates in a standard format. We have to convert the data into seconds, minutes, and days with a date reference sets on 01/01/1970. 
 ### 1.2 Changing the Category and Subcategory column to extract the data related to the plays
Louise is supporting a project for the creation of a play. We have to change the Category and Subcategory column in order to highlight the trend for the play subcategory. For a better reading of the database, we created two new columns, one for the categories, and one for the subcategories where we can filter on the plays results.
## 2. Presentation of the findings
### 2.1 Better success for the campaigns launched during summer
The analysis of the theater outcomes by launch date highlights that theater projects have a greater success rate when the launch date is during the month of May and June. 
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/85641189/123000630-6d1a3300-d375-11eb-8b02-2c383ba098f9.png)
January, March, September, and November have roughly the smaller amount of failed campaigns launched. The month of October has the highest proportion of failed campaigns launched. With the ambition to support the creation of the play "Fever", Louise should target the month of May or June to launch her campaign.
### 2.2 Projects with limited budget are successful
If we focus our analysis on the play subcategory, we highlight that the project with a budget below $14.999 have a greater rate of success. More than 50% of the plays are successful. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/85641189/123000687-81f6c680-d375-11eb-9291-8045168c95d5.png)
Projects with a budget over $45.000 are at risk with a higher rate of failure. Louise's project has a budget of $10.000. Though she has a higher probability of success.
### 2.3 Limitations of the dataset
Our client, Louise, is supporting the creation of a play. If we focus our analysis on the subcategory Play, we have a limited amount of data to work on. Our result might not be representative. 
In order to go deeper in our recommandations, we could have created a chart with Outcomes and the length of the campaign. If we already highlight that the fundrising campaign should be done in May or June, we do not have any insight on the relationship between the outcome and the duration of the campaign. We could also represent the successful projects with a budget lower than $15.000 by launch date. The objective is to confirm that the launch date has an impact on the success rate whatever is the overall budget of the project.  
