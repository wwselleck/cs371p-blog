---
layout: post
title:  "Week of Monday August 23rd"
date:   2015-08-30 7:10:00
categories: 
---
Sam Bradford went 10 for 10 for 121 yards and 3 TDs on Saturday against the Packers. Prepare to bow down to your Eagle overlords.

The actual content of the two classes so far has been fairly trivial so far for anyone who's written any program in a strongly-typed langauge, so I guess this first blog post will be about the process of making this blog. 

I'm currently hosting my personal website using Github Pages and Jekyll, so my `wwselleck.github.io` website is already being used (which is being redirected to my own domain name.) This made the process of setting up this blog a little bit more difficult than usual.

1. Instead of just making a new Github repository named `wwselleck.github.io` and putting the generated website in the `master` branch, I had to make a `cs371p-blog` repository and put the contents of the site in a special `gh-pages` branch. This was certainly more steps than setting up the user page, but not really any more difficult as long as you're capable of switching branches.

2. The real problem caused by this was that every path in the new generated Jekyll site was using an absolute path that assumed the site was at the root. So for example a generated path was `/images/me.png`, when what I really wanted was `/cs371p-blog/images/me.png`. My first, and in hindsight very poor, solution was to prepend `./` to each route, turning it into a relative path. This worked for the index, but blew up miserably when navigating to a blog post. I should have seen this coming for pretty obvious reasons (index and blog posts are on different directory levels), but it required very little brain work so...it was worth a shot.
I took a look at Piazza to see if anyone else was using a project page instead of a user page, and found someone who was using a Jekyll Now generated page. I took a look at its source code and saw this is the `_config.yml`.
{% highlight python %}
# If you're hosting your site at a Project repository on GitHub pages
# (http://yourusername.github.io/repository-name)
# and NOT your User repository (http://yourusername.github.io)
# then add in the baseurl here, like this: "/repository-name"
baseurl: "/cs371p-blog"
{% endhighlight %}

alskdfjaslkdfjasldklaskdjfasjnweu
_(that's the sound of me realizing I was making this way more difficult than it needed to be)_

I saw things that looked like `{% raw %}{{ post.url | prepend: site.baseurl }}{% endraw %}` scattered throughout the site, but just overlooked it as boilerplate that Jekyll generated. Adding a `baseurl` to `_config.yml`, and prepending it to all of my paths fixed all of my problems.

## Tip Thing of the Week
I used to worship weekly at the Church of Igor Minar, but I think I've fully hopped off of the Angular 2 train in favor of [Aurelia](http://aurelia.io/). After using Aurelia for a few weeks at work and then going through some Angular 2 guides, writing code for Aurelia was so much more straight forward while at the same time using less magic to get the job done. If you're at all into web application development, give it a look.