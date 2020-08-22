---
layout: post
title:      "From simplicity, to complex confusion, ending upon relief."
date:       2020-08-22 03:54:38 +0000
permalink:  from_simplicity_to_complex_confusion_ending_upon_relief
---

<!-- wp:paragraph -->
<p>For my most recent project at Flatiron School, I was tasked with creating a Rails Application from scratch. Fortunately there are so many pretty amazing tools out there that can help you easily get started and a lot of the hard stuff out of the way. I am so glad that our instructor worked really hard to be able to teach us about Devise even though it was not part of our curriculum. Devise makes setting up authentication for users a breeze. In fact it is so simple that you can install it in three easy steps:</p>
<!-- /wp:paragraph -->

<!-- wp:list {"ordered":true} -->
<ol><li>Add gem ‘devise’ to gemfile.</li><li>Run bundle install in terminal.</li><li>Run rails g devise:install in terminal.</li></ol>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>And that's it! You've now installed Devise! </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>After installing devise I decided to utilize if for a User model and again, the process was just another three steps in my case: </p>
<!-- /wp:paragraph -->

<!-- wp:list {"ordered":true} -->
<ol><li>Run rails g devise user in terminal.</li><li>Run rails db:migrate (to migrate user table).</li><li>Run rails g devise:views in terminal (optional).</li></ol>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>I chose to run the third optional step because I new I was going to need to be able to manipulate my views. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Tada!! Devise has now been fully set up within my brand new Rails app! By doing these six easy steps, I now have access to some really cool features that I now don't have to spend time on. Now I can focus on building out my other MVCs (models/controllers/views). </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Devise gives you some built in helper methods that are really helpful. My favorite was absolutely "current_user". </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Within my app I am able to check if the current_user owned a specific meal or dish thanks to the devise built-in methods coupled with methods I wrote. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>It all seems so simple doesn't it? And it is, and still my next steps were pretty simple as well. Thanks to my lessons at Flatiron School, and this website: <a href="https://www.adrianprieto.com/how-to-setup-devise-and-omniauth-for-your-rails-application/" data-type="URL" data-id="https://www.adrianprieto.com/how-to-setup-devise-and-omniauth-for-your-rails-application/">https://www.adrianprieto.com/how-to-setup-devise-and-omniauth-for-your-rails-application/</a>, I was able to set up Omniauth with Devise, and allow my users to sign-in via their Facebook page. Another great win in my book and a fantastic start to my project. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>After this I was able to easily run:</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">rails g resources</pre>
<!-- /wp:preformatted -->

<!-- wp:paragraph -->
<p>in my terminal and through that command I was able to easily create my migrations, controllers, models, and view folders. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>With all of this set up I was able to really dig in and begin my project. At times I very much wished the process was just written out step-by-step so that I could follow along. However, I am here to learn and having someone tell me how to do it all would not cause me to stretch my learning muscles. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I decided to base my Rails App Project off of the previous Sinatra App Project I had built. I figured this should be a pretty simple task. In my Sinatra Project our User had many Meals and the Meals belonged to the User. In my Rails Project it needed to become a little more complex so I had to change it up a bit. We still had a User, we still had a Meal, but this time I also added a separate model for our Dish. First, User has many meals, and Meal belonged to the user. Second, Dish has many Meals, and Meals belong to the Dish. And third, User has many Dishes, THROUGH Meals, and Dishes have many Users, THROUGH Meals. And just for a bit of clarifying, Dish = Food (Spaghetti), and Meal = Day/Time (Sunday, Breakfast). </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>This all seemed so simple to me and I figured it would only take me a day or so to complete. I knew that I would have to read with nested routing which meant that I would be coding a route from the meals in the app via a particular meal_path, using the meal_id from that particular meal and going to the dishes so that I could create a new dish that was tied to the particular meal I had already called upon. Although, that can seem pretty complex itself, I feel like that was pretty simple compared to the accidental mess I got myself into. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>We needed the nested routing, I new that, but the way I built my project and the only way I could seem to make it work the way I needed it to, was to also delve into nested forms. Meaning, not only did I have to build the forms for the nested route, I also had to nest another form within that form. Me, being so new to all of this, I felt, very much, as if I was in over my head adn no idea what I was doing on this one. I did not know how I was going to complete this. I had not learned this yet. Fortunately, I am not alone. Fortunately, I have Google. Fortunately, I have my lessons, instructor, and fellow students. Pooling all the resources I had available to me, I was able to complete the app, the nested routes, and even the nested forms. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I honestly have to say this was probably one of the hardest project I have ever done in my life, but I am so glad I was able to do it. Because of the confusion and times where I was stretching my brain to the max, I was even able to help others with similar situations. Building a Rails App mostly on your own in such a short time, is not an easy thing to do, but it definitely can be done and quite rewarding. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I'm sure I will continue to tinker more and fine tune as time goes on, but I definitely look forward to deploying the app and having my family actually use it when planning future multi-day events. </p>
<!-- /wp:paragraph -->
