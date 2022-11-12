# Kickstarting with Excel

## Overview of Project
An up-and-coming playwright, Louise, wants to start a crowdfunding campaign that can help fund her play called Fever.  She has estimated a budget of over $10,000 but needs help analyzing crowdfunding data.  To help her, I am organizing, sorting, and analyzing the crowdfunding data to determine if there are specific factors that make a project’s campaign successful.  Since Louise is now close to her fundraising goal, she would like to know how different campaigns performed in relation to their launch dates and funding goals. 

### Purpose
The purpose of this project is to create two analyses, one with outcomes based on launch date and one with outcomes based on goals. These analyses will help Louise mirror other successful ones in the same category.  

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date 
![deliverable #1](https://github.com/LLudivina/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)
With this graph, we can track the campaigns that were successful.  We can also track the campaigns that failed and the ones that were canceled. By considering the months, we can see on which specific month a campaign was the most successful.  In this case, it was within the month of May.

These months were extracted from the campaign dates found in the crowdfunding data.  However, the campaign dates were not readable.  
Hence a unix timestamp converter had to be used and this was one of the difficulties that I encountered during this part of the analysis.  The conversion of time from epoch dates to human-readable dates can be a bit confusing to use at the beginning. My approach was mainly trial and error. 

### Analysis of Outcome Based on Goals
![deliverable #2](https://github.com/LLudivina/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)
This graph shows the percent of campaigns that were successful, failed, or were canceled at a particular goal range. 

One of the difficulties I encountered when creating this graph was keeping track of the amounts. For example, a zero was sometimes left out during the calculation and this let to different values on the graph.  To overcome this problem, I had to double check the data at various time points during the calculations. 

### Challenges and Difficulties Encountered
There were a couple of challenges that had to be addressed after downloading the crowdfunding data.  The data was provided as a tabular data that had to be filtered, formatted, or made readable.  Any Unix timestamps data was first confirmed and then converted using the timestamp converter. I also used conditional formatting to prepare the data for the creation of visualizations.  By using Pivot Tables, I was able to create the first deliverable, the Outcomes Based on Launch Date graph.  The second deliverable, the graph titled Outcomes Based on Goals, was created using a simple line chart on excel. 

## Results
Based on the graph, Outcome Based on Launch Date, there are more successful campaigns than failed or canceled campaigns. This is a good indication for Louise.  To mirror a successful campaign, she should focus on campaigns launched in the month of May.  Overall, Louise should launch her campaign in the summer and avoid launching her campaign in the winter. 

Based on the graph, Outcome Based on Goals, Louise has a little under 60% chance of reaching her budget goal of over $10,000.

Aside the results, this project had some limitations in the data.  For example, the current data has information from different countries, but each subgroup is somewhat small. It would be helpful if data from a larger sample size could be provided. Also, the outcomes based on launch date graph could benefit from a unit on the y-axis. The graph shows 0 to 120, but that could be the number of individual people or millions of people.  Since I used the data, I know the value, but it may not be so clear to Louise or someone else.

Another graphs that can be created for this project is a bar chart to compare a successful vs failed campaign on a specific month.


