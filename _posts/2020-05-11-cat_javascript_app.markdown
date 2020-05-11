---
layout: post
title:      "Cat JavaScript App"
date:       2020-05-11 17:56:58 +0000
permalink:  cat_javascript_app
---


For my JS project, I created an app that animal shelters and cat cafes could use to display their animals. I used to work at a cat cafe, so I designed the app around the most common questions I would receive around the cats. People always wanted to know a cats personality type and we would get so many emails and phone calls asking. This gave me the idea of an instagram type layout, but when you upload the picture adding the option to select 8 different personality traits. The app I created display more information about a cat then you typically see on instagram (most cat cafes main way of communicating with the public).

Anyways, the app I created allows you to upload a picture of a cat with a name, age description, status, and you can select 8 personality traits. The hardest part of building this was creating the personality traits as a separate model that belonged to the cat model. I ended up creating an in-between model called cat_personality_traits to help with that. That created its own complications though. Through a lot of trial and error, I realized I had to create a cat_personality_traits_attributes= function in the cats model to get the objects to properly interact and belong to each other.

