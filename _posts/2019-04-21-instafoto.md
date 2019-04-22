---
layout: post
title:  InstaFoto
subtitle: Very basic Instagram-style blog
date:   2019-04-18 23:45:42 -0300
categories: project
link: https://insta-foto.herokuapp.com/
image: instagram-logo.png
tags:  
    - Rails
    - Heroku
    - Haml
    - CoffeeScript
---
Image by [ElisaRiva](https://pixabay.com/users/ElisaRiva-1348268/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=1834010) from [Pixabay](https://pixabay.com/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=1834010) -- many thanks! 

From Yonathan Ayenew's [8 Beautiful Ruby on Rails Apps in 30 Days & TDD - Immersive](https://www.udemy.com/8-beautiful-ruby-on-rails-apps-in-30-days/) -- Project 3. 

It's supposed to be an "Instagram clone" -- you can log in and post pictures that other users can comment on. I prefer the look of the "older" 3-column layout, so I've stuck with this for now.

### What I learned from this:
Back to Haml. I was having errors with both the CSS and the JavaScript that turned out to be Haml indentation errors -- that took me a while to discover! I initially assumed the JavaScript problems were because it's my first time doing anything with CoffeeScript, and I thought the CSS might not work because I was using a newer gem than he was, but they both turned out to be simple indentation errors.

I also used Cloudinary and Carrierwave to upload the images, since the gem he used is now deprecated. Cloudinary didn't pick up on the link in the .env file, and I still have no idea why! Eventually solved that by including the .yaml file, following their instructions, and it worked like a charm, including on Heroku. Must remember to change that on Heroku and see if it still works… Also, there was a problem with an "uninitialized constant" in PhotoUploader that mysteriously fixed itself -- see the blog post for 17 April.

### [On Heroku](https://insta-foto.herokuapp.com/)
