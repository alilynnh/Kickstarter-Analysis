# An Analysis of Kickstarter Campaigns
## Overview of Project

### Background
The client for this project was an up-and-coming playwright who wanted to create a crowdfunding campaign titled "Fever". In order to determine a budget for the client's campaign, data from previous crowdfunding campaigns was analyzed. Once a budget was set, the client successfully raised the goal amount in a short period of time.  
### Purpose
The purpose of the current project was to analyze the previous campaign data in order to compare the campaign outcomes in relation to their respective launch dates and monetary goals. The results of the analysis can be used by the client to make informed decisions about their future ventures, as well as compare their results to other campaigns.   
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
To begin the analysis of outcomes based on launch date, a pivot table was created with the following parameters: <!-- not sure if parameter is a good word, may change -->

| Parameter | Field Used |
| --------- | -------- |
| Columns | Outcomes |
| Rows | Date Created |
| Values | Count of Outcomes |
| Filters  | Parent Category & Years |

After creating the initial table, the dates were grouped by month and was filtered to only include theater campaigns. This resulted in the table below. 

<!-- Figure out how to insert image of table lol -->

Next, a pivot chart was generated with the months on the x-axis, the count of outcomes on the y-axis, and each outcome denoted by a differently colored line. This was done in order to visualize the breakdown of campaign outcomes for each month and to visually determine if trends are present. The chart can be seen below. 

<!-- Figure out how to insert image of chart lol -->
### Analysis of Outcomes Based on Goals
To begin the analysis of outcomes based on goals, a table was created with each row being a different goal amount category. The first category included goals less than $1000, and the subsequent increasing goal categories had ranges of $5000. The number of successful, failed, and canceled crowdfunding campaigns for plays were calculated for each goal category by using COUNTIFS statements. For example, to obtain the number of successful campaigns for plays that had goals from $1000 to $4999 was determined with =COUNTIFS(Kickstarter!$F:$F, "successful", Kickstarter!$D:$D, ">=1000", Kickstarter!$D:$D, "<=4999", Kickstarter!$R:$R, "plays").  
### Challenges and Difficulties Encountered

## Results
