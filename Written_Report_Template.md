# Kickstarting with Excel

## Overview of Project
Using the Kickstarter dataset to visualize campaign outcomes based on their launch dates and their funding goals.

### Purpose
Knowing how different campaigns fared in relation to their launch dates and their funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
We create a pivot table from the Kickstarter worksheet and filter it based on "Years" and on "Parent Category" to only show data for "theater". We also filter the column labels to only show "successful", "failed" and "canceled". We visualize the relationship between outcomes and launch month by creating a line chart from the pivot table. 

![Theater_Outcomes_vs_Launch.png](/Resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
We visualize the percentage of successful, failed, and canceled plays based on the funding goal amount. We create dollar-amount ranges so projects can be grouped based on their goal amount. We populate the "Total Projects" column with the number of successful, failed, and canceled projects for each row. We also calculate the percentage of successful, failed, and canceled projects for each row. We create a line chart to visualize the relationship between the goal-amount ranges and the percentage of successful, failed, or canceled projects.

![Outcomes_vs_Goals.png](/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
- Initially it was a bit tricky to figure out the correct syntax for the COUNTIF formula.
- COUNTIF formula was used for creating the dollar-amount ranges for grouping the projects which was than converted into a pivot table. But, in the pivot table the Row Labels were not sorted automatically because "Less than 1000" and "5000 to 9999" were not in the proper positions. These rows had to be manually sorted to be in the correct ascending order. 
- For outcomes based on goal the current data has 0 canceled plays but the sheet for the empty data still had to be created with the columns similar to successful and failed plays. Otherwise, the chart would not be generated correctly. 

## Results

### We can conclude the following from the Outcomes based on Launch Date:
- Based on the pivot table and line chart May is the most common month for successful theater outcomes.  
- Based on the pivot table and line chart May is also the most common month for failed theater outcomes.

### We can conclude the following from the Outcomes based on Goals:
- Hundred percentage of projects fail when the goal is between 45000 and 49999.
- Most projects are successful when their goal is less than 1000.

### Limitations of this dataset:
- When creating the pivot tables some amount of manual sorting and filtering is required. 
- For outcomes based on goal there are no canceled plays. Perhaps if the dataset included more years we could find some patterns for canceled plays.

### Some other possible tables and/or graphs that we could create:
- Apart from line charts, we could also create bar charts.
- We could create pivot table and graphs for theater outcome based on deadline
