# An Analysis of Kickstarter Campaigns

### Table of Contents
- [1 Overview of Project](#1-overview-of-project)
  - [1.1 Purpose](#11-purpose)
  - [1.2 Tools Required](#12-tools-required)
-  [2 Analysis & Challenges](#2-analysis--challenges)
-  [3 Results](#3-results)

## 1 Overview of Project

This analysis was originally conducted to assist a playwright, Louise, who was interested in starting a crowdfunding campaign to help fund her play, *Fever*. Excel was used to organize, sort, and analyze crowdfunding data to determine whether there are specific factors that make a fundraising campaign successful. Due to preliminary findings, Louise's play, *Fever*, came close to its fundraising goal in a short amount of time. 

### 1.1 Purpose 

Using insights derived from Excel, the purpose of this project is to help Louise determine how different campaigns fared in relation to their launch date and funding goals. Using the Kickstarter dataset, two technical requirements needed to be met to fulfill Louise's data request:

- Create an *Outcomes vs Launch Date* Chart
- Create an *Outcomes Based on Goals* Chart

### 1.2 Tools Required 

- Excel (version 16 or later)

## 2 Analysis & Challenges 

### Outcomes Based on Launch Date

Using a pivot table and graphing functionalities in Excel, a visualization was created to show campaign outcomes ("successful", "failed", and "canceled") in relation to its launch date. 

To create this chart, in the **Kickstarter** dataset, a *Years* column was added to the Kickstarter worksheet to extract the year from the *Date Created Conversion* column using the `YEAR()` function. A pivot table was created based on all the contents of the Kickstarter worksheet, including the new Year column. The table below depicts how the pivot table was properly structured to conduct this analysis: 

Filters | Columns | Rows | Values
------- | ------- | ---- | ------
Parent Category, Years | Outcomes | Date Created Conversion | *Count of* Outcomes

Once the pivot table is created, the parent category filter should be adjusted to only show results for the **Theater** category like the image below: 

![](images/pivot_outcomes_vs_launch.png)

Note, Louise is only interested in data for campaigns that already completed and are listed as either "successful", "failed", or "canceled" - ensure column labels do **not** include "live" campaigns.

## 3 Results 


![](images/theater_outcomes_vs_launch.png)

