# Kickstarting with Excel

## Overview of Project

Using the Kickstarter dataset provided, this challenge is to analyze how successful different kickstarter campaigns are in relation to their launch dates and their funding goals. The output will be a written report with two charts. 

### Purpose

Analysis of Kickstarter campaigns by launch dates and funding goals. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Starting with the Kickstarter Excel file, I created a pivot table to summarize outcomes by month of launch date. My first attempt, I used Year as the row field but after looking at the example provided, I realized that I needed to use the Date Created Conversion Date instead. Once the pivot table was correct, the next step of creating the line chart was pretty straightfoward. By default, the button text appeared on my chart, so it took me a few minutes to figure out how to remove those. I selected a preset style that had the line markers since those were shown in the example. The result is the chart below.

---

![Outcomes Based on Launch Date](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

For the second analysis, I created a new sheet to add formulas for counting the Kickstarter data based on criteria. I used the CountIf and Sum functions. I remembered from class that the $ is used as a lock character, and that made copying the formulas across columns easier. I didn't know that before bootcamp started, so I learned something new! Since the Number Cancelled was all zeros, that surprised me so I took a minute to filter the data to double check that that was true. And I checked against the images in the material to make sure I didn't miss something. The result is the chart below.

---

![Outcomes Based on Goals](/resources/Outcomes_vs_Goals.png)


## Results

- Theater campaigns launched between May and July were more successful, and those months had more campaigns launched total. December is not a good month to launch a Theater campaign.
---
- Regarding the impact of the goal amount, goals should be under $40,000 as the success rate falls steeply for amounts over that. 
---
- The data used for the analysis is for launch dates from 2009 to 2017, which is probably a reasonable range but is not necessarily predictive of the future. There is a Currency column in the file and it's not explicitly labeled if the goals and pledged are already converted to US dollars. If the column header specified, it would be clear.
---
- For the Outcomes Based on Goals, I only analyzed the Theater category since that was the purpose of this activity, but it might be useful to see if the same trends are true for other categories.
