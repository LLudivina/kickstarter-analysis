# Kickstarting with Excel

## Overview of Project 
For this module 1 challenge, we were tasked with helping Louise analyze crowdfunding data. Louise is an up-and-coming playwright who started a crowdfunding campaign to fund her play called “Fever”.  Since Louise is now close to her fundraising goal of over $10,000, she would like to know how different campaigns perform in relation to their launch dates and their funding goals.  To help Louise, I downloaded the dataset workbook host file provided to us and created a local file that could be more readable and searchable with excel tools. In the end, I was able to examine the crowdfunding data to determine if there were specific factors that make a project’s campaign successful.

## Purpose
The purpose of this project was to organize, sort, and analyze crowdfunding data to provide Louise with a visual analysis of campaign outcomes based on their launch dates and campaign outcomes based on their funding goals.  This way, Louise could launch a successful campaign by mirroring other successful campaigns in the same category.

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date 
First, let’s look at the data for campaign outcomes based on their launch dates.  Figure 1 shows a pivot table with data from the kickstarter worksheet located in the local file that I had previously downloaded and renamed to KickStarter_Challenge.  I then used filters to select the theater category and extract the months from the original launch dates. Furthermore, Figure 1 shows data for the theater category that was arranged by months and one of three labels: successful, failed, or canceled. For example, a filter for the theater campaign category for the month of January resulted in 56 successful, 33 failed, and 7 canceled ones.

**Figure 1**

![Figure 1](https://user-images.githubusercontent.com/115508896/202921935-ae5cacbe-07f9-49d2-abe5-f494982f4f92.png)

A better visualization of the data can be found in Figure 2, which shows the relationship between outcomes and launch month.  This deliverable was created using a simple line chart on excel.  By using conditional formatting, I was also able to provide Louise with information at a glance. Based on the line graph, we can see on which specific months the campaigns were the most successful. In this case, it was early in the year and within the month of May.

**Figure 2**

![deliverable #1](https://github.com/LLudivina/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

As mentioned before, the months seen in both the pivot table (Figure 1) and the line graph (Figure 2) were extracted from the campaign dates found in the original source file. However, the campaign dates were not readable, so any Unix timestamps data was first confirmed and then converted using the timestamp converter. This was one of the difficulties that I encountered during this part of the analysis. The conversion of time from epoch dates to human-readable dates can be a bit confusing to use at the beginning. My approach was mainly trial and error int terms of tracking the allowed input for batch convert. 

### Analysis of Outcome Based on Goals
Moving on to the second part of the Analysis, we will look at the process for the analysis of outcome based on goals.  Using the original source file, we created a new sheet titled outcomes based on goals. A range of goals was listed on the first column while the second, third, and fourth columns were filled in using the COUNTIFS () function on excel.  The SUM () function was then used to obtain the results for column five.  The percentages for the last three columns were also calculated.

**Figure 3**

![Figure 3](https://user-images.githubusercontent.com/115508896/202922064-07d50247-1897-4e9e-92bf-0a2e699882a3.png)


**Figure 4**

![deliverable #2](https://github.com/LLudivina/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

Figure 4, shows the percent of campaigns that were successful, failed, or were canceled at a particular goal range.  This line chart helps visualize the relationship between the goal amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis. 

One of the difficulties I encountered when creating this graph was keeping track of the amounts. For example, a zero was sometimes left out during the calculation and this let to different values on the graph. To overcome this problem, I had to double check the data at various time points during the calculations.

### Challenges and Difficulties Encountered
There were a couple of challenges that had to be addressed after downloading the crowdfunding data. The data was provided as a tabular data that had to be filtered, formatted, or made readable. The unix timestamp converter was a bit hard for me to use since it was my first time using this type of converter. Excel was more manageable due to my exposure of the software in previous classes.  Learning to create my repository in GitHub was also a bit tricky to do. Hopefully, I managed. 

## Results
Based on the graph, Outcome Based on Launch Date, there are more successful campaigns than failed or canceled campaigns. This is a good indication for Louise. To mirror a successful campaign, she should focus on campaigns launched in the month of May. Louise should avoid launching her campaign in the winter.  Based on the graph, Outcome Based on Goals, Louise has a little under 60% chance of reaching her budget goal of over $10,000.

Aside the results, this project had some limitations in the data. For example, the current data has information from different countries, but each subgroup is somewhat small. It would be helpful if data from a larger sample size could be provided. Also, the Outcomes Based on Launch Date graph could benefit from a unit on the y-axis. The graph shows 0 to 120, but that could be the number of individual people or millions of people. Since I used the data, I know the value, but it may not be so clear to Louise or someone else.

Another graph that can be created for this project is a bar chart to compare a successful vs failed campaign on a specific month.



