---
layout: post
title:      "One Project At A Time - Michael McCullough"
date:       2019-08-15 11:03:41 -0400
permalink:  cli_data_gem_-_park_trails
---

#CLI Data Gem - Park Trails



   For this CLI project I built an app that would list the Palm Beach County nature trails, and when requested, provide additional information about each individual trail.   If I am being honest I was intimidated by this one; I had roughly two months of total coding experience when I started and this was also the first time I needed to write code that wasn’t guided by TDD.  It was an incredible learning experience and when completed, provided the reference point I needed to realize how much I have truly learned in these last two months.

   Within my project I build three classes: CLI class, Trail class, and Scraper class.  I began by creating a functioning CLI with hardcoded data just to make sure that the CLI flowed smoothly.  Next I built the Trail class which was as simple as creating an initialize method to instantiate a new trail with the information returned from the Scraper class.  Both of those classes were pretty much straight forward and simple to build, the Scraper class however, was not.  Conceptually I understood what the scraper needed to do and how to build it, but once I began scraping the information, the return values really took me for a ride.

   Scraping in this project presented significantly more problems than I anticipated.  For me, there was such a disparity in difficulty between the course labs and this project.  During course labs we scraped HTML that was provided by Flatiron, it was somewhat complex, but it was clean which allowed me to scrape it with minimal speed bumps.  The Palm Beach County website on the other hand, was a bit of a nightmare.  When iterating through classes and elements to pull the necessary info, I was returning elements with no text, text of a single element consisting of two different topics, and other issues.  After many hours of headaches I was finally able to return the info I needed and exclude the excess nonsense that was causing the issues.  

   I truly understand why Software Engineers are referred to as “problem solvers.”  I was able to persevere through this project by solving each problem that arose, one at a time.  It was tedious, but very rewarding.   Considering the fact that I had absolutely no coding knowledge two months ago, I feel very proud and validated in my accomplishment. 
	

