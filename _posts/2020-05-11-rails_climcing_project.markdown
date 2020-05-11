---
layout: post
title:      "Rails Climcing Project"
date:       2020-05-11 14:15:38 -0400
permalink:  rails_climcing_project
---



For my rails project, I created an app that allows to track and log climbs. Once a log is recorded you can see the other logs for that route. You are also able to leave comments on your own and other peoples posts.

The hardest part of this project for me was getting the facebook login to work. I ran into many issues and it broke my code a lot of times. One of the first issues I had was "user_id null for nill class" because of how I had set up my "current_user" method. By adding an "if statement" I was able to overcome this error, but from there more problems arised. The next issue I had was even though I could sign in and create user through facebook, I wasn't able to create a session. I later realized I had to manually create a secession ID in my Users::OmniauthCallbacksController. I eventually got it all working, but that was the hardest part of the project and what I sent the most time on.

