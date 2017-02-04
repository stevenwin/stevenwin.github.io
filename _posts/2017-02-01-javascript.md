---
layout: post
tag: personal
title: JavaScript Hell
---

I‘ve been struggling with JavaScript for a while now and initially, I felt as though I‘d never grasp the language.  The past few weeks of learning felt as though every topic lead to a deeper rabbit hole which required devoted attention.  Frustration was the norm as I would continually run into bugs after bugs, unable to understand why certain mechanics didn't work.  But I kept at it, day in and day out, and I can appreciate the progress being made.

I‘m grateful to have found a project to fully devote my JS learning time on.  During my time learning Python, I made the mistake of only reading and completing exercises in the book.  This methodology only made me better at completing individual puzzles, but it never helped me deconstruct problems on a whole and piece them back together.

The project I'm working on, on paper, is fairly simple.  I‘m using the UFC's and Fightmetric‘s API to pull all of the past events and fighters from each event.  From there, I‘m running a scraper to grab the relevant information for each fighter through Sherdog.  After all of the information is compiled, I‘m doing some calculations to predict the winner.

Fairly simple.

Except it‘s not.  It‘s not simple because going into JS, I was still stuck on a different programming paradigm that Python and Ruby taught me.  As I made my way through JS without any guides, I quickly learned that JS operates in a very different way.  JS operates asynchronously.  What this means is that as opposed to Python, where each line is executed chronologically, JS is able to request certain information from external sources on the side while it runs through the rest of the program.  The external information is “called back” to another function only after the request is complete.

This ability to “asynchronously” collect information really gave me trouble during the past few weeks.  I didn‘t know how to deal with information being collected and returned at random times.  I wanted to gather the UFC information before running Fightmetric, but I was never certain which result would pass back to me first.  This uncertainty messed up my program flow and I was stuck trying to hard code certain timers into the program.

After pinpointing this deficiency in learning, I spent several days trying to understand the inner workings of JS.  Why does it operate a certain way?  After reading through a dozen articles on the issue, I now have a much better understanding.  To deal with asynchronous data, JS has a clever technique involving the use of “callback” functions.  Callback functions are declared functions that are called upon once a certain declared criteria is met.  Understanding this helped me pass along information in a more logical manner for interpretation and I‘ve just crossed a big hurdle in completing this project.

I feel much more confident and hopeful about my programming journey now and I need to remind myself that there‘s always light at the end of the tunnel.  The only thing that‘s needed is curiosity and perseverance.