---
layout: post
title:  "Week of Monday August 30th"
date:   2015-09-06 06:00:00
categories: 
---
If you're in the mood to cry about the things you haven't done with your life (and let's be honest, probably never will), the new [Beach House album](https://open.spotify.com/album/35vTE3hx3AAXtM6okpJII) is pretty great. Some people on the internet have had the audacity to say it's a disappointment compared to Teen Dream, Bloom, and even Devotion, but in my inarguably correct opinion it's at the same level as the rest of their discography.

So this week I worked a bunch on the Collatz project, but haven't really spent a ton of time on it. I became familiar with Travis CI, issue tracking, Jekyll, and most of the non-C++ specific tools over the summer while working on front-end web developemnt, so I figured the majority of this project wouldn't be too difficult. I was only somewhat correct.

I only know the basics of vim and am too lazy at the moment to learn ssh more in-depth, so I took some time to try and set up a development environment for this class on my Macbook. Homebrew made the majority of that process go smoothly, the one major exception being getting Google Test to work. I had about 0 familiarity with using C++ libraries before this project, so I had to do quite a bit of Googling to get it to cooperate. Most of the tutorials had pretty similar instructions for getting gtest installed on a Mac, but for some reason after doing some magic compiling and then magically copying the magically compiled files into some magical folder that the project files magically have access to, I was still getting an explosion of errors when running `make test` on the Collatz project. At this point I needed to clear my mind, so I listened to Depression Cherry and cried only a tiny bit. I did some more Googling with the errors I was experiencing and didn't find much, but did notice multiple people mentioning that compliing the library and project with different compilers could cause such errors. I redid the gtest magical installing process again, this time running `export CXX = g++-4.8` before compiling, and it worked. Well kind of, I was still getting errors, but they were unrelated. :thumbs-up:. 

###Tipamajigger of the Week
I really don't like using tools and such blindly without at least having an adequate knowledge of how they work, so during that depressing installation process I read [this article](http://computers.tutsplus.com/tutorials/homebrew-demystified-os-xs-ultimate-package-manager--mac-44884) on Homebrew. It's not very in depth, but it helped me understand the output of Homebrew way better. I suggest you do too. Or not. I can't really force you. :simple-smile:.

