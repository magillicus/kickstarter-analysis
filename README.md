# Kickstarting with Excel

## Overview of Project

My client, Louise, has completed fundraising for her play entitled "Fever." Louise now needs my expertise to determine how related campaigns from the past fared in relation to their corresponding launch dates and funding goals.

### Purpose

By completing analysis on trended data from past play campaigns, Louise will be able to draw insights from the analysis to assist her in making informed decisions about when her "Fever" play should be launched and whether or not her funding goal is appropriately budgeted for maximum success.

## Analysis and Challenges

The first portion of the analysis was centered around identifying the level of success of past similar projects based on their launch dates. Subsequent analysis highlighted which projects were successful, unsuccessful or downright canceled based on their reported funding goals. While challenges were minimal, I did note an oddity that I will discuss below.

### Analysis of Outcomes Based on Launch Date

The first thing I did was create a pivot table to illustrate how many past campaigns succeeded, failed and were canceled based on the month of year the campaigns were launched. I filtered the campaign type (indicated as Parent Category) to show only theater campaigns, which is the campaign category type most closely aligned with Louise's project. 

Theater Outcomes Pivot Table by Launch Date 

<img width="314" alt="Theater_Outcomes_Pivot_Table_by_LD" src="https://user-images.githubusercontent.com/92264929/138844726-2b6bac77-f764-48e1-a046-edaedbb177da.png">

Afterwards, I created a line chart to compare the trends of successful campaigns to those that were both unsuccessful and those that were canceled over the course of the calendar year, stratified by month.

Theater Outcomes vs. Launch Line Chart

<img width="289" alt="Theater_Outcomes_vs_Launch" src="https://user-images.githubusercontent.com/92264929/138845110-2b4feee5-ac2b-425e-ad1a-123513f45432.png">

### Analysis of Outcomes Based on Goals

In this portion of the analysis, I first created a table with data indicating the number of successful, failed and canceled play campaigns
based on several tiered goal ranges. 

Outcomes vs. Goals Table ![image](https://user-images.githubusercontent.com/92264929/138844010-6f1e195c-2cb6-496b-bcda-6dce07512390.png)

By utilizing functions in Excel, I was able to calculate the number of play campaigns in each goal
tier for each outcome, labeled as either successful, failed or canceled. I also calculated the total number of projects in each goal tier, as well as the
percentage of those projects in each outcome category, organized by goal tier. I subsequently created a line chart to illustrate the trended outcome 
percentage data for each goal tier range. 

Outcomes vs. Goals Line Chart

<img width="241" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/92264929/138845488-e97311a5-6975-42a2-91ec-bddaa0f72b23.png">

### Challenges and Difficulties Encountered

The only issue I encountered was during the Analysis of Outcomes Based on Goals section (directly above) while creating the first table. The challenge instructions 
indicated that the listed tiers should be organized into 12 separate and labeled rows with clearly identified goal ranges. The final goal ranges, "45000 to 49999" and "Greater than 50000" technically do NOT include the value of $50,000. There were 4 data points in the "Number Failed" column with an exact value of $50,000. These data points need to be included in the analysis. I considered modifying the Goal range to read, "50000 or Greater," which would have been more accurate and inclusive of the four "$50,000" data points that technically should not be included if the row is to be labeled as "Greater than 50000." Instead, I just changed my function for the values of the "Greater than 50000" row to read greater than OR equal to 50,000, so as to include those four "$50,000" data points. "Greater than 50000," technically, does not include "$50,000," so the correct function should NOT include "or equal to" and should contain only a greater than symbol...but that would have been leaving out four important data points. To get full points for the assignment, I elected not to change the row title, but instead to include the ">= 50000" in the corresponding functions for that row instead of the indicated "greater than 50000."

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

According to my line chart, May appears to be the month with the most successfully launched campaigns, and success rates tend to steadily decrease afterwards. Additionally, May also apears to be the month with the most failed campaigns...which means that most of the playwrights elected to launch their plays during May, regardless of the outcome. However, the difference between the number of campaigns that were successful and those that were not was the greatest in May, indicating that while chances are the highest for both success and failure during that month, the likelihood for a successfully launched play is also at its highest.

- What can you conclude about the Outcomes based on Goals?

According to my line chart, campaigns with goals less than $1,000 are the most likely to be successful. Conversely, projects are the least likely to be successful when the funding goal is greater than $45,000.

- What are some limitations of this dataset?

When analyzing outcomes based solely on goals, there are no play campaigns with canceled outcomes. Consequently, there is no data to suggest or support that canceled shows are affected by funding goals at all. There is, however, data to support trends in canceled theater campaigns based on launch date. One cannot draw parallels between the two variables because outcomes by launch date are specific to a broader category, theater, while outcomes based on funding goals are specific to a more granular subset of data, plays.

- What are some other possible tables and/or graphs that we could create?

We could create a pivot table and/or chart that illustrates the correlation between play outcome and the number of backers behind the pledged funding, regardless of the pledged amount.  We could also see if there are correlations between the length of time a campaign runs (date ended - date created) and its overall outcome.
