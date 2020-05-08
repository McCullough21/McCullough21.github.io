---
layout: post
title:      "Javascript Project"
date:       2020-05-08 23:52:06 +0000
permalink:  javascript_project
---



As an avid golfer I utilize my Golf Handicap and Information Network “GHIN” application regularly to keep track of my handicap.  For my single page Javascript project I thought it would be fun to create an app with similar functionality, utilizing a Javascript/html/css frontend with a Rails api backend.  The app will allow a user to track their scores and will calculate the users handicap index based on those scores.  It was an interesting process for me.  Having been brand new to code when I started this bootcamp, I have been building on my knowledge base as the course has progressed.  This was the first time I needed to construct an app with a separate frontend and backend.  The only real challenge that I ran into was my lack of understanding regarding the JS event loop. 


	I knew that JS code ran asynchronously, but I did not fully understand what was  happening behind the scenes.  I realized I had an issue when attempting to make a POST request with fetch().   When a user enters a new score, I need to POST the data to the API to persist in the database; then retrieve the updated data with a GET request to re-render the page reflecting the new score and re-calculated handicap.  The problem was that my GET request was not returning the newly updated data.  After numerous failed attempts, I pulled up google.  I learned that during the event loop when an async function is executed it is set aside while the rest of the call stack executes, only returning to the stack once the promise returns and the call stack is empty.  What I didn’t know, or had forgotten, was that I needed to use the “await” keyword on my POST request to halt the call stack until the promise is returned allowing the GET request to retrieve the newly persisted information.

