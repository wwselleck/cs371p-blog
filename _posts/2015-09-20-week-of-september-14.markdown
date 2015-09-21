---
layout: post
title:  "Week of Monday September 14th"
date:   2015-09-20 011:00:00
categories: 
---

So...the Eagles suck again. :(.

This week my partner and I started work on Project 2, and it became clear very quickly that the actual solution to the problem would be extremely more difficult than last project's problem. Our schedules haven't allowed us to work on it for more than about 3-4 hours so far, so I don't really have too much to say about it yet. 

I guess the most interesting programming-related thing I did this week was learn more about how shell configuration works and get a decent setup working for my dotfiles. The first thing I did was make a `~/dotfiles` folder and copy over my `.bash_profile` and `.vimrc` files into it, and then of course set up [version control](https://github.com/wwselleck/dotfiles) for it. Then I made a very simple [bash script](https://github.com/wwselleck/dotfiles/blob/master/install.sh) based off of [Oliver's](https://github.com/oliveratutexas/dotfiles/blob/master/make-symlinks.sh), which basically just backs up the dotfiles in `~` and then copies over the files from the repo into `~`. So far I've used this repo and script to get the same configuration on my work, school, and personal machines with very little issue. 

## Tippy and the Sunshine Band of the Week
I switched to ZSH from bash just because I was curious, and so far I'm very happy with the switch. I used [Oh-My-Zsh](https://github.com/robbyrussell/oh-my-zsh) to get it set up and in just a few steps my terminal went from pretty lame to pretty schweet. The default OMZ installation has a git plugin that includes a pretty invaluable autocomplete feature which has made switching branches at work (with very verbose names) way easier. 