# Kickstarting with Excel

## Overview of Project
An up-and-coming playwright, Louise, wants to start a crowdfunding campaign that can help fund her play called Fever.  She has estimated a budget of over $10,000 but needs help analyzing crowdfunding data.  To help her, I am organizing, sorting, and analyzing the crowdfunding data to determine if there are specific factors that make a project’s campaign successful.  Since Louise is now close to her fundraising goal, she would like to know how different campaigns performed in relation to their launch dates and funding goals. 

### Purpose
The purpose of this project is to create two Analyses, one with outcomes based on launch date and one with outcomes based on goals. These analysis will help Louise mirror other successful ones in the same category.  

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date 
![deliverable #1](kickstarter-analysis/resources/Theater_Outcomes_vs_Launch.png)
One of the difficulties that were encountered during this part of the analysis was the conversion of time from epoch dates to human-readable dates.  It can be a bit confusing to use the converter.  My approach was mainly trial and error. 

### Analysis of Outcome Based on Goals
![deliverable #2](kickstarter-analysis/resources/Outcomes_vs_Goals.png)

Double checking the data was one of the difficulties that were encountered when creating this graph.  A zero was sometimes left out during the calculation.  This let to different values on the graph.  To overcome this problem, the data was double checked at various time points during the calculations. 

### Challenges and Difficulties Encountered
There were a couple of challenges that had to be addressed after downloading the crowdfunding data.  The data was provided as a tabular data that had to be filtered, formatted, or made readable.  Any Unix timestamps data was first confirmed and then converted using the timestamp converter. I also used conditional formatting to prepare the data for the creation of visualizations.  By using Pivot Tables, I was able to create the first deliverable titled outcomes based on launch date found in the next section.   The second deliverable titled outcomes based on launch data can also be found in the results section. 

## Results
Based on the graph, there are more successful campaigns than failed or canceled campaigns. This is a good indication for Louise.  To mirror on a successful campaign, she should focus on campaigns launched in the month of May.  Overall, Louise should launch her campaign in the summer and avoid launching her campaign in the winter. 

Based on the graph, Louise has a little under 60% chance of reaching her budget goal of over $10,000.

In terms of limitations of the data, it would be helpful if data from a larger sample size could be provided.  The current data has information from different countries, but each subgroup is somewhat small. 

When it comes to the deliverables, the outcomes based on launch date could benefit from a unit on the y-axis. The graph shows 0 to 120, but that could be the number of individual people or millions of people.  Since I used the data, I know the value, but it may not be so clear to Louise or someone else.



