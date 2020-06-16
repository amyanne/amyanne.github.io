---
layout: post
title:      "How to Build a Checkbox Form in JS with Ruby Backend"
date:       2020-06-16 21:59:55 +0000
permalink:  how_to_build_a_checkbox_form_in_js_with_ruby_backend
---


This image has an empty alt attribute; its file name is check-box.png
Here is a tutorial on how to build a checkbox form in HTML and JavaScript and how to have it communicate with a Ruby backend to persist the data.

*I used the gem rack-cors to allow my backend and frontend to communicate*

Ruby Backend
For this project I set up a ruby backend. I created three models: cat, personality trait, and cat personality trait. A cat has many cat personality traits through personality trait and has many cat personality trait. Cat personality trait belongs to the other two models. Personality trait has many cats through cat personality traits (read about more active record associations). 

This image has an empty alt attribute; its file name is active-record-1.png
This image has an empty alt attribute; its file name is active-record-2.png
This image has an empty alt attribute; its file name is active-record-3.png
The cat personality trait model works as a link between cat and personality trait. I decided to seed the 8 personality traits into the data base because I didn't need the code to be flexible and it was an efficient way to allow to the frontend to easily persist data in the backend.

In my cats model I build a custom accept_nested_attributes for cat personality trait.

This allowed me to get the name of the personality trait and append it to an array instead of getting two ids. 

HTML
The html is where I build the checkbox form. 

This image has an empty alt attribute; its file name is form-1.png
This image has an empty alt attribute; its file name is form-2.png
﻿

﻿

﻿

This was part of a larger form so I put the personality traits in a <field set> to group them together. The id="trait_name" allows us to access the form in our JavaScript code to see if a box has been checked. 

JavaScript
I created a function  to see if the box had been checked, if the box had been checked I appended it to a new array. 

This image has an empty alt attribute; its file name is javascript.png
Then I called that function in my function that gets all the data from the form.

This image has an empty alt attribute; its file name is javascript-2.png
I created a submitCat event that calls the getCatFromForm function to get the data to then call the cat constructor to build the cat. 

This image has an empty alt attribute; its file name is js-3.png



