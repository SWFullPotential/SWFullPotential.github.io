---
layout: post
title:      "A Gem?!? Is it shiny?!!!"
date:       2020-06-17 21:25:58 -0400
permalink:  a_gem_is_it_shiny
---

<!-- wp:group -->
<div class="wp-block-group"><div class="wp-block-group__inner-container"><!-- wp:paragraph {"backgroundColor":"background","textColor":"foreground"} -->
<p class="has-foreground-color has-background-background-color has-text-color has-background">Finally, we are here! At the end of the first module of my Software Development Bootcamp! I feel like we just started, yet so much has happened in the meantime. During orientation when we started this cohort, our educational coach showed us this chart. I guess you could call it a chart. It showed the journey of becoming a Flatiron Graduate. Where when the student first starts they are all excited for what is about to come and can't wait to begin. Then as you go along you encounter something confusing and realize this might actually be hard. You start to doubt yourself and and some start to slip into the depths of despair and begin to believe they can't do it. The way I perceived things when she told us this, was that this was over the course of the entire program, but i'm realizing that is not entirely true. Based on what I just experienced during this first module, I wonder if we will go through these same cycles, yes "despair" included, for each module?? Boy, I hope not!</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>This module has been challenging for two reasons. I am very new to this industry completely, first of all. And second of all, the knowledge I had prior to this program was in JavaScript, not Ruby. Switching my brain to a different programming language while in the middle of getting used to another was difficult. I had times where I would say aloud, "They're just making words up!!" I had times where I was really ahead, and then times where I actually got behind. It was a bit of a roller coaster, but finally we are here at our first Portfolio Project. The CLI Data Gem Portfolio Project. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>"OOOOh! A gem!!!" Will it be shiny? Will it sparkle? Is it going to glitter when the sun hits it? Oh, wait, did you say a "Data Gem"? What on earth is a "Data Gem"? Well, a gem in Ruby language is basically a neatly packaged little ruby program ready for you to use. Different gems do different things. Some gems are the entire runnable program, and some are used to aid you in building a gem of your own.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>When users run this program, or gem, they will be able to interact with data through a CLI(Command Line Interface) program. My job was to find an API that I wanted to use and write the code necessary to interact with the API, obtain the data, convert it into usable objects, and create a fully functioning CLI.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Now, the CLI Data Gem that I created  uses a Harry Potter API which you can find at: potterapi.com. It is free to use, but if you really want to get access to the majority of the data, you need to create and account and get an access key. After getting the access key I took the information from the API(Application Programming Interface) which was given to me as an array of hashes and converted them into an array of objects so that I could use them in my program. After creating the environment I needed to build my project, I began to code.</p>
<!-- /wp:paragraph --></div></div>
<!-- /wp:group -->

<!-- wp:heading -->
<h2>Building the project out: </h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>First, I started by working on the API code so that I could get the information I was needing for my CLI. I used RestClient to get the data from the PotterAPI site I was using and JSON to format the information from the responses into an array of objects. Once I had the objects and finished iterating through the data I was able to use them in my CLI.</p>
<!-- /wp:paragraph -->

<!-- wp:group -->
<div class="wp-block-group"><div class="wp-block-group__inner-container"></div></div>
<!-- /wp:group -->

<!-- wp:image {"id":40,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://swfullpotential.files.wordpress.com/2020/06/image-3.png?w=1024" alt="" class="wp-image-40"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>The next step was to build out my "Spells" class: </p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":42,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://swfullpotential.files.wordpress.com/2020/06/image-4.png?w=881" alt="" class="wp-image-42"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>I knew there was going to be a new object for each hash within the array that was given by the API and I knew what information was going to be received. Within my spells class I was able to create an initialize method that would create each new instance of the spells class, the objects. I needed each object to be put into an array so I set my variable @@all to an empty array and shoveled each new instance of spells into that array using my save method. I also created an all method so that I could call up the entire array. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>From here I began to work on my CLI, but honestly at this point I was bouncing around from API, to Spells, to CLI like crazy. I'm not going to include all of the CLI because frankly, it's just too long. You can look at it on GitHub later. Yes, I'll include the link. In the CLI, I created a run method that I call in my executable file. This method shows the user a welcome message and asks them kindly to wait while the data is loaded. In this method I also call my API.get_spells method and this is where the data is loaded into the program for the user to access. The next thing I created was the method to print the menu: </p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":43,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://swfullpotential.files.wordpress.com/2020/06/image-5.png?w=816" alt="" class="wp-image-43"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p> Once this is printed the user gets to actually interact with the program. They either choose a number for a category, or the exit the program. To make this work I used "if" statements. These are great functions within ruby. If the statement isn't true, it just moves on to the next statement, and this keeps going until a statement within the method is true. Then the program will do what ever the true statement calls for. </p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":45,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://swfullpotential.files.wordpress.com/2020/06/image-6.png?w=1024" alt="" class="wp-image-45"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Instead of using "if" in the middle of "if" statements we use "elsif", but if there is an "elsif", there MUST be an "else" as the last statement to check. In the picture above you can see that the "else" statement is for any invalid user entries. This protects the user and brings them right back to the main menu. </p>
<!-- /wp:paragraph -->

<!-- wp:group -->
<div class="wp-block-group"><div class="wp-block-group__inner-container"><!-- wp:paragraph -->
<p>The final part of the CLI is to exit the program and the main menu has instruction for ending the program. </p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":47,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://swfullpotential.files.wordpress.com/2020/06/image-7.png?w=1003" alt="" class="wp-image-47"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Thank you for taking the time to read my post for my first project! I am proud of it and would love for you to check it out and play around with the program. You can find the repository here: <a href="https://github.com/SWFullPotential/potter_api_052620">https://github.com/SWFullPotential/potter_api_052620</a>. Thanks again and happy coding!</p>
<!-- /wp:paragraph --></div></div>
<!-- /wp:group -->

<!-- wp:group -->
<div class="wp-block-group"><div class="wp-block-group__inner-container"><!-- wp:group -->
<div class="wp-block-group"><div class="wp-block-group__inner-container"></div></div>
<!-- /wp:group --></div></div>
<!-- /wp:group -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->
