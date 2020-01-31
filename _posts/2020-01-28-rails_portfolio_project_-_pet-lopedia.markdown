---
layout: post
title:      "Rails Portfolio Project - Pet-lopedia"
date:       2020-01-28 15:40:54 -0500
permalink:  rails_portfolio_project_-_pet-lopedia
---


The App

	For the Rails Portfolio Project I decided to create an app that would provide users with information regarding dog breeds. The idea to create this app came from my own experience with my wolfdog Nola.  Before I decided to commit to a wolfdog puppy I was instructed by the breeder to research and learn as much as I could about them.  I read a few books and spent countless hours on google reading all about their behaviors, training, and generally what to expect when owning one.  What I really took note of was that the best information came from random wolfdog owners who wrote about their own experiences raising their pups.  With that in mind I created, “Pet-lopedia.”  Within this app a user can learn about general traits and characteristics of different breeds, but can also follow it up with first hand accounts from users who own those breeds. 
Coding Process	

	 Before I started this project I felt like I would fly right through it.  I felt totally confident in my ability to meet all requirements: MVC structure, associations (has_many, belongs_to, has_many_through), nested forms, nested resources, partials, and omniauth.  As you might imagine though, that confidence was quickly tested as I began construciton.  Something will always break or misbehave, but no problem occurred  that I was unable to overcome on my own.
	Whether it was during the construction of my nested forms, nested resources, or omniauth setup; I was always able to work through hangups with: 
	
raise ____.inspect	
	
By far the most useful debugging tool was using “raise” and “inspect” to debug and track the flow of information throughout the app.  The most difficult problem I faced was setting up third party authentication with omniauth.  The information that was passed from the third party, in this case Facebook, was complicated and I struggled to figure out why I was not receiving the proper values.  Once I raised and inspected the auth hash I realized why I was extracting the UID but not the email.  Email was in an [“info”] key.

auth['uid']
auth[‘info']['email']

