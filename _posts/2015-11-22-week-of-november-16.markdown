---
layout: post
title:  "Week of Monday November 16th"
date:   2015-11-22 20:00:00
categories: 
---
The Eagles got thoroughly smushed by a(nother) crappy team and I don't want to talk about it... :(.

This week my partner and I finished up Project 5, and my inkling that it would be significantly easier than Project 4 was actually correct. Project 5 was a lot like Project 4, just...simpler. Like I mentioned last week, I think the biggest differentiator between Life and Darwin was that in Life, the cells only really cared about themselves. The cells needed to know how many alive neighbors were around them (and in the case of the Fredkin Cell, in which direction), but the actions they performed were only on themselves. In Darwin, however, the creature would possibly have to do something to another cell, like infect it or hop onto it, which added another layer of complexity. Creatures had to have some access to the board they occupied, and there weren't really many clean ways to give it this access while still maintaining a good OOP design. 

I went a pretty straightforward route to accomplish this by sending the Creature an instance of the Darwin board it lived on with every call to "execute" (or whatever I called it), and the coordinates of itself. The Creature then took those coordinates and the direction it was facing (stored in Creature) to calculate the coordinates of the space it was facing and send all of that information off to Species to do the actual execution. Species then took allllll of that information and forwarded it to whichever Instruction (kept in a list of Instruction objects) was next. The Instruction object "handle" method then did the actual execution of the instruction on the Darwin object using the two pairs of coordinates. 

In Life, we had one pass through the board that generated all of the "alive neighbor" counts for each of the cells, and then another pass to call "evolve" on each cell. That's it.

So problem solving wise, Project 5 was significantly easier than Project 4. The added complexity of Project 5 was the inheritance and Cell wrapper class stuff which, while certaintly not easy, was a much easier problem to solve than the design problem of Project 4. After reading some SO and Piazza posts about the cloning pattern, it was just a matter of translating the pattern over to Life. It really doesn't matter since I don't think Prof. Downing is trying to make each project harder than the last one, but I personally did find Project 5 to be easier than Project 4 by a decent margin.

### Auntip Anne's Pretzels
_(I, having literally 1 internship's worth of CS career experience, feel icky trying to give career advice, but I'm doing it anyway because I think this one is relevant to people at my level of experience)_

After doing a bunch of work on a personal project and putting it on your resume, make sure you don't just abandon it immediately and never look at it again. I made a web app over the summer and was asked in an interview this week about the design of the back end, and my panicked answer was something along the lines of "It umm accepts API requests and is pretty simple and responds with JSON". To be fair to myself, it is a pretty straightforward back end that does actually nothing cool (unless you think fulfilling basic API requests is cool), but if I had actually looked at that project more recently than 3 months ago I might have been able to put it in less stupid terms. 