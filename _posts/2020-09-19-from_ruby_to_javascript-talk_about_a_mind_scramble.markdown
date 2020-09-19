---
layout: post
title:      "From Ruby to JavaScript-talk about a mind scramble!"
date:       2020-09-19 20:27:44 +0000
permalink:  from_ruby_to_javascript-talk_about_a_mind_scramble
---


<!-- wp:paragraph -->
<p>When I first began my Software Engineering path, before starting at Flatiron School, I started with The Odin Project. It was really great and a lot of what I started with was JavaScript. So when I began at Flatiron School I figured the JavaScript section would just be cake for me. Oh how wrong I was! After spending the pas three months completely immersed in Ruby world, transitioning to JavaScript was a struggle, to say the least. Thre were many times where my brain would begin to write code for my JavaScript project and realize it won't work,  because I was actually coding it out with Ruby syntax. Learning Ruby was hard enough, but I never thought I would get to the point where I just wanted to go back to Ruby, yet there I was wishing for Ruby. Of course, now that I have finihsed my JavaScript project, I feel more comfortable with it, but I do wish the basic JavaScript section was more than just one month. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>When the JavaScript module began things seemed easy, but then there was a lot of jumping around. It seemed like there was no nice flow. There are so many ways you can achieve the same results by using JavaScript and even different flows for each. I learned with my JavaScript project working feature by feature was the best approach for me. I had not been coding like that in the past with Ruby. In Ruby I would work through the models, then the controllers, and the finally the views. With JavaScript I had to totally re-order my process. I have to plan ahead through the entire project almost before I could even begin. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I decided, for my JavaScript project, that I would base my single page application on my last profession. I am a licensed cosmetologist and used to have my own salon. I decided I would create a page where I, as the stylist, could list the services I offer and the prices associated with them. This meant I had a "has-many/belongs-to" relationship. A hairstylist has many services they offer, and each service with it's price, belongs to the hairstylist. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The first feature I decided to build was the "index" page. I had to create the Ruby on Rails backend and seed in some basic starting data into the database. Once I was able to view the JSON results of the data I knew I would be able to render the proper information on the JavaScript front end. I chose to have the services nested within the view of the hairstylist data. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>After completing the backend, the real work began. To begin I needed to link the front end and the back end together so I set the URLS as constants that I would be sending fetch requests to. Since I was working on being able to view the existing data my first focus was being able to fetch the data and display it to the user/viewer. It was a struggle to keep myself away from defaulting back to my Ruby brain where I would just create the view and write out the HTML with both HTML and Embedded Ruby. Instead I used JavaScript commands and functions to create the nodes that would be viewed on the front end. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>After creating the initial view that would be seen by the user/viewer, I decided to change my focus to the delete function. Sometimes a hairstylist will change what they offer so the would need to be able to delete a service. This function seemed pretty simple to create, but I was also reminded the importance of ordering my lines of code in a particular order. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The next feature I decided to focus on was creating the form where the hairstylist would be able to create a new service to add to their list of offerings. Thanks to my ability to work with others I learned a much simpler way to create the HTML needed to build the form. I chose to leave both ways in my project instead of keeping them all the same because I wanted to show that I know how to do both. Also it gives me the opportunity to go back later and remember different ways to accomplish the same goal. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Next I brought my focus to the function of actually adding the new service. This was the most challenging part of the project for me. I was able to create the new service in the back-end from the front-end, but it wasn't showing up on the front end unless I refreshed the page. I knew that was not acceptable so I kept pushing and trying every way I could figure out. I sought help and a few of us struggled together trying to figure it out. Finally I was able to find the help I needed. It turns out that when I initially fetched the data from the back end, I also needed to create a JavaScript object of each of the services, and I wasn't doing that. Once we figured that out, I ran into another problem. Too much logic was happening because I mistakenly was trying to re-render pretty much the whole page each time I added a new service. This meant that after adding three services I ended up with three forms on the page. The fix was simple, instead of re-rending that much I only needed to re-render the list of services. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Finally, I put all my focus on styling the page. This was also a difficult shift for me because am used to doing inline CSS instead of creating an additional CSS page to render. It look quite a bit of googling, but I knew I would be able to figure it out. It was a bit of a frustrating process, but I am really glad I was able to style a different way than I was used to . I learned a lot and am now very proud of how the end result turned out. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I tell you what, they were not kidding when other students said this was both the most challenging and rewarding experience of their lives, they were not kidding. This has been extremely difficult for me, but I am learning so much!</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>If you'd like to check out the finished project here is the Github link: https://github.com/SWFullPotential/Stylist_Offerings_JS </p>
<!-- /wp:paragraph -->
