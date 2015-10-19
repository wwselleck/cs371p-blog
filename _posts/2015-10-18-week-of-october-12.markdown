---
layout: post
title:  "Week of Monday October 12th"
date:   2015-10-18 20:00:00
categories: 
---
The Eagles haven't played yet, but the Mets are 1-0 in the NLCS, so at least I have that going for me.

I missed Monday's class, for which I am throughly ashamed. Although it seems that, for some reason, a lot of people missed Monday's class, so I feel a little less ashamed. This week my partner and I started Project 3. At first we thought it might be the easiest one yet, at least easier than Project 2, but after an hour or so of work it became clear that that wasn't the case. Code-wise this project doesn't seem too difficult, but figuring out a good solution is going to take some time. We've worked on it for around 5-ish hours total and are just now getting to allocate(), so we probably still have about 10 hours or more to go. 

While working I became very aware of how little documentation exists on gcov. And by little documentation, I mean about 5 short pages on the GNU website and some Stack Overflow questions. It turned out that our 1.5 hour problem was just us not realizing that TestAllocator.c++ would also give a report for Allocator.h and had nothing to do with our compliation setup, but nevertheless, should an actual gcov problem come up I have no confidence that there will be any documentation that's very helpful.

## Einstein Tip Bros
I did a lot of vimming again this week, and along the way came across a bunch of interesting articles and guides that help you understand how vim works, especially for configuration. Here are some of them...

+ [Debugging vimrc](http://vim.wikia.com/wiki/Debug_unexpected_option_settings)
+ Running `:h startup` gives an overview of what happens when you start up vim
+ [A Good vimrc](http://dougblack.io/words/a-good-vimrc.html)
+ [Stack overflow question about autoload](http://superuser.com/questions/668886/why-isnt-the-scripts-in-my-autoload-folder-being-executed-in-vim)