---
layout: post
title:      "My Sinatra Project"
date:       2020-07-22 02:02:02 -0400
permalink:  my_sinatra_project
---


<!-- wp:group -->
<div class="wp-block-group"><div class="wp-block-group__inner-container"><!-- wp:paragraph -->
<p>When I learned about the Sinatra project I would need to do, coming up with an idea was actually pretty easy! We needed to have users that could log in and have many of something. That something needed to belong to the user. Comically enough, I had just experienced something that described just that. My family had planned and was about to go on a family reunion camping trip. Instead of each family bringing food for each member of their subfamily for each meal, each day, we decided it would be better if each family picked a day and meal that they would prepare for everyone. The "many" part comes in because there were more meals that needed to be prepared than there were families attending. It was perfect!</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>I set up my Sinatra App using Corneal (https://github.com/thebrianemory/corneal). By doing that I already had the MVC set up! MVC breaks down the different parts of a Sinatra App. First, we have Model. The models are the Ruby classes. In my project, I had two models, the user, and the meals. These can represent the data and can include helper methods that scope down through the active record query methods. Next, we have View. The views are all the different embedded ruby files that hold all of our HTML. These are the files where we code what we want the user to see, like the login page, the sign-up page, etc.. Finally, we have Controller. The controllers are where we create the routes that will be taken. It is our relay system, the data from the browser to the app, and the app to the browser.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Within the controllers, the RESTful routes are written. A RESTful route is where you map out the route between the HTTP verb and the CRUD actions. There are eight different RESTful routes, but within my Sinatra Project, I only used seven. The seven used within my meals_controller are:</p>
<!-- /wp:paragraph -->

<!-- wp:table -->
<figure class="wp-block-table"><table><tbody><tr><td><strong>HTTP Verb</strong></td><td><strong>RESTful Route Used</strong></td><td><strong>CRUD Action</strong></td><td><strong>Purpose</strong></td></tr><tr><td><strong>GET</strong></td><td>‘/meals’</td><td>Index (Read) Action</td><td>Our index page where we can see all the meals.</td></tr><tr><td><strong>GET</strong></td><td>‘/meals/new’</td><td>New Action</td><td>Where a new meal form is showed to be filled out.</td></tr><tr><td><strong>POST</strong></td><td>/meals’</td><td>Create Action</td><td>Creates a new meal.</td></tr><tr><td><strong>GET</strong></td><td>/meals/:id’</td><td>Show (Read) Action</td><td>Displays the meal based on the meal ID.</td></tr><tr><td><strong>GET</strong></td><td>/meals/:id/edit’</td><td>Edit Action</td><td>Gives the form and meal to be edited by meal id.</td></tr><tr><td><strong>PATCH</strong></td><td>/meals/:id’</td><td>Update Action</td><td>Where our meal is updated based on it’s id.</td></tr><tr><td><strong>DELETE</strong></td><td>/meals/:id’</td><td>Delete Action</td><td>Deletes a meal based on the meal id.</td></tr></tbody></table></figure>
<!-- /wp:table -->

<!-- wp:paragraph -->
<p>Above I mentioned “CRUD Action”. What is CRUD? CRUD stands for: create, read, update, and delete. Create is where we are creating a new instance of the class. Read is pretty self-explanatory, but it can be done by showing all or by showing one at a time for the viewer to read. Update can be done in more than one way as well. We can completely replace the object or update certain elements of an object. Finally, we have the delete action, again, very self-explanatory, this is where we delete an object. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>In my Sinatra project, I was also able to practice and learn more CSS and HTML skills. I had both frustrations and fun with this part of the project. I have more of a creative mind so the CSS (styling) is where I tend to bite off more than I can chew. I have dabbled in CSS a little bit, but it was a while ago so some cobwebs had to be dusted off first. It took some time to get my brain to shift to CSS language vs Ruby and Sinatra, but I managed to come up with something that both worked and I liked. Not too plain, but not too crazy either.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Here is the link to the GitHub repo so you can check it out for yourself: <a href="https://github.com/SWFullPotential/SinatraProject_AndersonGatheringFoods">https://github.com/SWFullPotential/SinatraProject_AndersonGatheringFoods</a>.Eventually I will also deploy it through Heroku so that my family can actually utilize it. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>All in all, I did enjoy this project and look forward to actually using this app to help my family with future events.&nbsp;</p>
<!-- /wp:paragraph --></div></div>
<!-- /wp:group -->
