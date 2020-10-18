---
layout: post
title:      "The Final Project-React/Redux"
date:       2020-10-18 20:20:29 +0000
permalink:  the_final_project-react_redux
---


<!-- wp:paragraph -->
<p>Wow! We are finally here! The final project! </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Mod five has come and just about gone. I thought jumping from Ruby to JavaScript was a mind scramble, but working with React and Redux has been an entirely different ballgame. The stress of learning two frameworks within a one-month-long module has been pretty intense, but I can finally say I've successfully created a functioning React-Redux App. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p> The cycle started much the same as every other project  with “OH boy, what on earth am I going to do for my project?!” Then, naturally, in the middle of a yoga sesh, this CRAZY idea pops into my head. I think how cool it would be to create something like that and the more I think about it the more I wonder if it would meet the project requirements, but regardless of whether or not it does, my mind begins to wander, no PLUMMET down the rabbit hole of ideas and features that could be created and more and more ideas blossom. I can see in my mind how it COULD look when finished and the animations that COULD be added to create a really cool user experience. The excitement bubbles up and begins to reach the top of my pot and suddenly boils over into a wave of “OH SHIT this is WAY too much to do in a week!!!!” and the panic sets in and the imposter syndrome becomes all too real….“There is NO WAY I can do this”, “It’s way too much to do and WAY too much CSS “, “I better start thinking of something else”….WAIT!!! I remember that I am in control and I CAN break this down. I sit my butt down barf it all out on my screen, break it down, see what the project requirements ARE, analyze piece by piece and see that, holy shit….this MIGHT actually work…. I MIGHT actually have a plan to create the minimum viable product AND a plan to extend it further already in place. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>So I sent the plan to my cohort lead and asked if he thought it would work. I nervously began the project before hearing back from him because it was the weekend and I knew he was busy, but I needed to get started. Fortunately, he said it could work! I dug into two articles sent to me by a fellow student. First: "User Authentication in React via Rails API", by John Guest, <a href="https://medium.com/swlh/react-reactions-cfdde7f08dff">https://medium.com/swlh/react-reactions-cfdde7f08dff</a>, which helped me begin the set up for the user side that I wanted my project to have. Followed by the article written by the student who suggested the first article: "Dealing With Redux User Authentication &amp; Flatirons Final Hurdle", by Daniel Andrew, <a href="https://medium.com/swlh/dealing-with-redux-user-authentication-flatirons-final-hurdle-cbf2d7638d1f">https://medium.com/swlh/dealing-with-redux-user-authentication-flatirons-final-hurdle-cbf2d7638d1f</a>, which linked the authentications to redux and actually taught me how to get it functioning. With the help of these articles and live help from Dan and my cohort lead Enoch I was able to create a working User interface for my project. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>After getting that to work, I was able to focus on the purpose of my app, a Daily Tarot reading app. Now mind you, I personally don't do tarot readings, but I happen to have a friend who is a reiki master and she does tarot readings. I've always found the process interesting but recently becoming a bit of a minimalist I didn't see the value in carrying around decks of cards, SO I thought it would be cool to create an app that carries the cards for you and you can still get/do your reading. Several people voiced concerns about building such an app saying things like, "I don't think it works that way...", or "don't you need a certain juju to do a reading?". I put quite a bit of research into tarot readings for this project and learned some interesting things. I learned that anyone can do a tarot reading and those who do tarot readings for others, frequently do readings for themselves. Therefore, this could actually work as an app. I also learned that there are already apps similar to mine already out there, but I purposely did not look at those other apps because I did not want to cloud my mind with others' ideas. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Now, back to my freak out in the beginning. I have so many ideas for this app, but with only having a short amount of time to build it, I knew I would have to only create a minimum viable project. Once you create an account and log into the app, you are given two choices. You can either navigate to all of the cards or to the daily reading section. When a user navigates to either choice, a fetch call is sent to the Rails API backend I created, to grab all of the cards in the deck. When you click on all cards you are greeted with the list of cards which are each a link. The link will take you to the details of each card, including the meanings both up and reversed (the meaning is determined by which way the card is drawn). A user can view each card and become familiar with the entire deck. This is important for someone who wants to do readings, you need to know your deck. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The daily reading link brings you to a view that reminds the user to relax and breathe before drawing a card. It is important to focus your energies before doing a tarot reading. On that page, there is a button for drawing a card. The function that is called when the button is clicked, is simulating a random draw from an actual deck. Only one card is drawn for a daily reading. When the button is clicked one card will be shown to the user with the matching card image either up or reversed. The meaning associated with that card and direction is displayed as well for the user to read and interpret.  </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>This app has the potential to become so much more than it already is. I already have plans to add features for additional types of draws such as 3-card draw, 6-card draw, and Celtic Cross Draw. All of these are typical types of draws. I also plan to add a function that saves and logs daily draws so that the user can go back and look at their history. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>It has been a challenging process creating stateless components, containers, and properly wiring in thunk so that asynchronistic calls are possible. I have been able to use my knowledge of Rails, JavaScript, React, and Redux in one little project. I went from thinking I was going to run out of time, to realizing I actually do know what I'm doing and creating a working project. The styling side again was a challenge, but I'm getting better and better with CSS and am happy with the current state of the app. I can still see how this project can evolve and am so excited to continue creating my vision for this application. I look forward to the continued challenge and even am challenging myself to learn React Native after graduation to turn this into a mobile app. </p>
