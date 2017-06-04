---
title: Let's get relational
author: Rick Gilmore
date: '2014-09-03'
slug: let-s-get-relational
categories:
  - science
tags:
  - open science
  - Databrary
---

We know that [Databrary](http://databrary.org/) will have to compete against other data sharing services. Those of us who really enjoy building products and providing services that help others don't like to talk about competing, but it's a fact of life. Our project has generous support from [NSF](http://www.nsf.gov/awardsearch/showAward?AWD_ID=1238599&HistoricalAwards=false) and [NICHD](http://projectreporter.nih.gov/project_info_description.cfm?aid=8531595&icde=15908155&ddparam=&ddvalue=&ddsub=&cr=1&csb=default&cs=ASC) now, but that's no guarantee about the future of the project. We have to deliver a service that meets researcher's needs. But, rather than worry about how Databrary can compete against Dropbox or Box or Amazon to provide cloud storage, we're doing something else. We're building a system that does what no other data sharing service I know about does -- understands experimental design.

When I say understands, I am speaking loosely, of course. What I mean is that rather than provide a simple, flat-file storage service, we're building a system that can represent the structure of the studies we hope researchers will store with us and eventually share. Databrary's "back end" is a relational database that allows researchers to store and share research data in a structured way. Most developmental scientists, indeed most research psychologists, take measures from participants at particular places and times. Databrary's data model enables researchers to upload information about the settings (place, time, who conducted the study), participants (age, sex, race, ethnicity, and other person-specific variables), and measures (tasks, behaviors, questionnaires, physiological recordings, etc.) that are involved in behavioral research. Databrary keeps that information intact and structures it for visualization and for search. This means that we have to build ways for researchers to upload their data in ways that are familiar to them, like spreadsheet-like interfaces or multi-track timelines for temporally dense data streams like videos or eye-tracking. It also means we have to store the relationships between data elements, including their temporal relations -- what happened when -- in powerful and flexible ways that will enable others to use the data in the future.

We think the effort building this system is worth it because it will enable comparisons across studies to be made by future researchers in ways unimaginable to investigators today. Databrary is building for the future, and that means we're getting real relational today.