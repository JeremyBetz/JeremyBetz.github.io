---
layout: post
title: MTA Turnstile Analysis and Metis Week 1
---

#Metis:

Today was the start of my second of twelve weeks as a data science student at Metis in Chicago. Throughout the program I'll be working on five data science projects as I learn some of skills necessary to be an effective data scientist
data science bootcamp. The curriculum for week one included python libraries: pandas, matplotlib, and seaborn.

#MTA Turnstile Analysis:

**The Task**

In only one week, We've already completed our first data science project. Our hypothetical problem involved optimizing the placement of street teams in NYC so that an organization promoting women in technology could maximize exposure and generate funding through a gala event.

**The Data**

The NYC Transit Authority has publicly available data on turnstile entries and exits at subway stations across the city. We used the four more recent weeks of turnstile data with the hope of predicting foot traffic in NYC using the data on subway station entries over the period.

**Exploratory Analysis**

Initially, we aggregated the data for unique turnstiles into stations and plotted total turnstile entries per station over the entire period. When the result indicated relatively low values for some popular Manhattan stations, we were forced to look at the data set further and remove several values that seemed to have been recorded in error. Our new data set no longer had the same number of data points for each station so all future analysis was done with average ridership for the available data during a given time period.

Repeating the initial analysis with the newly cleaned data using average ridership rather than total ridership yielded more intuitive results so we preceded to further analyze some of the top stations. When deciding how many stations to analyze we looked at the average daily ridership for each station and found that a substantial break existed between the tenth and eleventh stations followed by relatively little change such that the top ten stations had nearly as much traffic as the next twenty.

We preceded with the ten stations with the highest traffic and looked at average ridership by weekday for each of the stations rather than across the entire four week period, all of which resided in Manhattan. Across all of these Manhattan stations, we found a pattern of high traffic from Monday through Thursday followed a clear drop on Friday and significantly lower numbers on Saturday and Sunday. We reasoned that commuters made up a large portion of subway ridership in Manhattan so a drop was to be expected, but the size of the drop and the consistency across relevant stations meant we focus only on canvassing those top Manhattan stations from Monday to Thursday.

**Moving Forward**

While we were able to take data from nearly 400 subway stations and give a recommendation of stations and days of the week to canvas, the MTA data could be further used to break down each station by time of day. It may also be worth considering weekdays separately across the entire data set to check for stations that normally have low ridership but may experience time periods of peak ridership that compete with the top stations. We expected that the additional complexity of including more stations in the canvassing, but only during select periods, would not be worth the gain in ridership when one must consider the logistics of moving around teams during the day, but it is possible that exceptional periods exist for some stations that may warrant the additional complexity.

Additionally, incorporating additional data that can address expected contribution in addition to total traffic, may improve the model's ability to address the second objective of funding the organization rather than focusing on the objective of exposure. Ideas to consider include socioeconomic data by location to address financial ability to contribute and data on profession demographics to target people already involved in tech and students hoping to enter tech so that interest in the cause is captured in the model. Traffic volume can address exposure, but targeting interested parties and those with the means to contribute would likely improve funding for the organization.
