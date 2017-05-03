---
layout: post
title: Modeling the Impact of Home Advantage in Football and Metis Week 3
---

# Football Match Analysis:

**The Task**

For my second [Metis](https://www.thisismetis.com/) project I was asked to build a linear regression model using data scraped from the web. My initial plan was to build an alternative *Expected Goal Difference* metric for evaluating team performance in a football match. *ExpG* is normally calculated independently for each team in a match using their shots taken and the long term conversion rates from each location, but I wanted to see how other match statistics correlated with goal scored including opposition statistics.

**The Data**

Because of the value of football data, it can be hard to find data that is both easily available and free. The best source I found for building my model was [whoscored.com](https://www.whoscored.com/) who have match summary pages for numerous leagues. Using Beautiful Soup and Selenium, I was able to scrape team statistics related to passing, shooting, dribbling, tackling etc. for the 2015/16 Premier League, Bundesliga, and La Liga seasons. The three leagues had a combined 1066 matches during the season.

**Exploratory Analysis**

Using the match data I built a linear regression model with a target of home team goal difference (home goals - away goals) using features from the [whoscored.com](https://www.whoscored.com/) match summary page. [whoscored.com](https://www.whoscored.com/) have far more potential features than necessary and several of them have very high multicollinearity so feature selection was important. One common calculation of time of possession, for instance, is the ratio of passes completed by the team to total completed passes in the match.

From the potential features list, *shots on target*, *total touches*, *completed passes*, and *errors* were found to have a statistically significant impact on the expected goal difference for both teams. That is, home team *shots on target* correlated positively with home team *goal difference* and away team *shots on target* correlated negatively with home team *goal difference*. *Total touches* also had the same direction of correlation while *completed passes* and *errors* correlated in the opposite direction for both sides. All of these correlations seem to follow common sense with the exception of *completed passes* which one might assume correlates positively with goals, but when you control for touches and shots, better chances tend to come from quick counter attacks rather than considered attacking moves. It seems that excessive passing has a negative correlation with goal difference for a team.

Along with those symmetric features, the model also had several statistically significant asymmetric features for the home team that were not statistically significant for the opposition. *Shots off target*, and *corners* for the home team had a negative correlation with *goal difference* while shots off the *woodwork* and *blocked shots* correlated positively with home team *goal difference*. In other words, the model punishes the home team for taking speculative efforts that are *off target* or created from *corners* rather than seeking quality chances; Away sides don't receive the same punishment. I expect that this is because home sides are often more capable of creating quality chances so the opportunity cost of a speculative effort is much higher than it is for away sides who must often take the chances they are given. When an away side shoots from an ambitious position, they may not be forgoing the opportunity to create a better chance, whereas the home side cedes possession unnecessarily with speculative efforts.

**Moving Forward**

Initially I built this model using only data from the 2015/16 Premier League season but the results surprised me so I expanded from 380 matches to 1066 to see if the significant features remained asymmetric. I would like to continue to expand the size of the data to see if the results hold, but significance held on the complete dataset. Additionally, I would like to consider more specific match features such as the location of touches, passes, shots etc. and pitch characteristics for a match such as dimension and surface type considering the current model suggests a difference exists between home and away sides. Perhaps pitch variation can account for why home sides seem to find success in different ways to opposition

Additionally, I would like to see how *expected goal difference* works as a predictor of future match results in a similar way to current applications of *ExpG* as a feature of predictive models for football results.
