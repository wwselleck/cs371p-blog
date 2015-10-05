---
layout: post
title:  "Week of Monday September 28th"
date:   2015-10-04 22:00:00
categories: 
---
The Eagles actually looked decent, but still lost to the Redskins.

I can't really think of a whole lot that went on with this class this week. We don't have any projects going on, and there weren't any guest speakers. I guess I'll just give my thoughts on the class so far.

#### The Good

I'm definitely learning a lot, despite already being fairly familiar with some of the course's major tools (Github, Travis CI, issue tracking, etc.) I knew essentially no C++ going into this semester and feel like I've become at least somewhat competent at it. At least competent for the kind of programming we've had to do in this course. The things we go over in lecture are also interesting, and I definitely learn a lot in them every time even if I'm already familiar with what we're going over that day. And Prof. Downing's teaching style of calling on people randomly definitely works, assuming its purpose is to make you pay attention like if your life depended on it.

##### The Questionable

I don't want to say "The Bad" because I, someone with give or take 2.5 years of programming experience, feel pretty stupid trying to criticize the way someone with decades of experience teaches a class. But everyone is entitled to their opinion no matter how wrong it is, so I'll give it.

For being an Object-Oriented Programming class, I don't feel like I'm learning all that much about object oriented programming. Aside from the book readings, the majority of the class feels like an industry and C++ crash course. The topics we cover in lecture, albeit interesting, are usually either fairly C++-centric or seem to have very little to do with OOP. Maybe I'm off-base with this, but I fail to see how unit testing, exceptions, and lambdas are so essential to learning OOP that they deserve their own day(s). 

The other gripe I have is with how industry-centric the course is. I am very aware of the benefits of pair programming, issue tracking, continuous integration, etc., but that's not what I'm taking this class to learn. It would take me 3 times as long to formulate these thoughts into paragraph form, so I'm just gonna start listing...

+ I had a great partner for Project 2 and having him definitely lessened the work load quite a bit, but I think doing the entire thing on our own would have been a much better C++ learning experience, for both of us. In my 2 years at UT, I feel like the points where I learned the most were in 312, 314, and 429 when I was forced to do a project all on my own. I get that it's not required to have a partner, but I'm sure most people who really care about their grades don't see it that way. 

+ I spent probably around 25% of my time on Project 1 just being paranoid that I had set my repo up correctly to conform to the incredicly detailed instructions on what can and can not be in it. I'm assuming these very strict rules are supposed to mirror industry, where your story implementation needs to match the acceptance criteria exactly. Again, I get it, but it seems overly strict for a class that is supposed to be about OOP. Speaking of trying to mirror industry...

+ It would be apparently be a great tragedy if I committed my Doxyfile and someone who cloned my repo was able to generate documentation for it using the same settings I did. Given the emphasis this class puts on developing software like it's done in the real world, I find it very surprising how backwards some of the project criteria is. In general with source control, you don't commit files that are generated dynamically, and instead commit the files you need to do that generation. For example, you don't commit Babel-transpiled ES5 code to your repo, but the ES6 source code and build file needed for the transpiliation. Or in this situation, you don't commit generated documentation and instead just commit the Doxyfile needed to generate it. 

It probably seems like I hate this class given the size discrepancy between those two sections, but I really do enjoy it and am learning a lot. And like I said, Downing obviously has megatons of experience more than I do, so I'm inclined to trust his judgement over mine. In fact, I'd love for someone to read this and tell me why I'm completely wrong on one or all of these points. 

### Tippy the Kid
I spent a lot of my week writing a Reddit bot in Javascript, and have now decided that that was stupid and am instead going to write it in Python. The asyncyness of Javascript is great most of the time, except in cases where I want it to just STOP DOING SOMETHING FOR LIKE ONE SECOND PLEASE. I'm currently drowning in promise spaghetti because of this. This actually isn't a major problem because the solution is already available using Babel and ES7 [async-await](http://www.sitepoint.com/simplifying-asynchronous-coding-es7-async-functions/), which allows you to write asynchronous code in a synchronous style, but I'm just going to use this as a Python learning opporutunity instead.