---
layout: post
title: The NHL API
---

### Topic and Findings 

[This](https://jkburrows.github.io/Project-1/) is a link to the vignette for my NHL API project. The github repo for this project is [here](https://github.com/JKBurrows/Project-1). 

For this project, I created an R function that contacts a few of the endpoints from the NHL’s stats and records APIs. Then I created a few plots and tables to explore the data. 

One finding I made is that some endpoints from the stats API don’t return what the documentation sites ([records](https://gitlab.com/dword4/nhlapi/-/blob/master/records-api.md), [stats](https://gitlab.com/dword4/nhlapi/-/blob/master/stats-api.md)) led me to think they would return. In particular, when contacting the teams endpoint of the stats API, the *person.names* modifier and the *statsSingleSeasonPlayoffs* modifier return the same information as the unmodified endpoint. They don’t seem to modify it at all. 

Another finding I made is that penalty minutes appear to have a stronger negative relationship with a team’s win percentage during the regular season than during the post season. In my vignette, I speculate that this is because, during the post season, players are better at fouling strategically. 

A third finding I made is that the NHL has more teams with a winning record than teams with a losing record. Perhaps this is because losing teams tend to go out of business. 

### What would you do differently in approaching the project?

If I did the project again, I would create an outline first to plan out what I want to do. This was my first time trying to query a moderately complicated API, so I didn’t know enough about the process to create a plan beforehand. But now that I am more familiar with the process, I think that pre-planning would be helpful. 

Also, if I did the project again in real life instead of for a class, I would like to independently validate my data. That would mean finding someone else who has also taken the time to query the NHL’s APIs and comparing data with them. 

### What was the most difficult part of the logic and programming for you?

Two difficult parts of the programming were: 

* The length of the functions involved. Some of them were so long that it was easy to get lost while writing them. It was easy for my eyes to get lost, and it was easy to lose my train of thought. 
* Flattening the data. Querying the APIs often returned nested objects. Writing code to un-nest them was time consuming. 

### What are your big take-aways for future projects?

Honestly, the biggest take-away is that all this takes is practice. If I did a similar project for the NFL’s API tomorrow, it would go much faster. And if I did the NBA after that, it would go even more smoothly. 

Another take-away is that it is easier to make meaningful plots and tables when you have a question in mind that you want to answer. For this project, I had a lot of NHL data, but no real motivating question about the NHL that I was trying to answer. 












