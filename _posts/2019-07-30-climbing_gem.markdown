---
layout: post
title:      "Climbing Gem"
date:       2019-07-30 15:46:09 +0000
permalink:  climbing_gem
---


I build a gem that scraps from a website, receiving the 100 most popular climbing routes and returns route, location, or grade based on user input. 

My process for completely this project was to break everything down to parts. I started with building my scraper class (arguably the most challenging part of the code). I originally started with Nokogiri's parsing code doc.css, but I quickly realized that wouldn't work. After some experimenting I decided to use xpath. I coded in a counter into that code collect all bits of raw data. From there a built a method that cleaned up and formatted the data and put it in a hash.

Next, I started building my routes class. It was pretty simple. It took in the hash that the scraper class and created an instance of each route associated with a name, grade, and location. This class was also responsible for the code that would find routes by location or grade.

Last I built my CLI class. This part was the easiest to create. I built my menu and command options. Then I built my run class. Building this was a little bit of trial and error, but it come together the quickest.

