---
layout: base
title: "Using Bootstrap CSS with Jekyll"
---

# Using Bootstrap CSS with Jekyll

There are multiple ways to integrate [Bootstrap](http://getbootstrap.com/) with [Jekyll](http://jekyllrb.com/) 
for Github Pages. In this article I'm gonna show how to get it done fast and clean :). 

I think using something like Bower or NPM is a good practice and of course convenient. In the project directory
type **bower init** to initialize bower.json file then for installing bootstrap or whatever you want to install
type **bower install package_name** (here it is _bower install bootstrap_) then you can use bootstrap CSS and JS in 
your html files using link and script tags. **But** there is a subtle issue here, in order to serve bootstrap 
in Github Pages you should **avoid** ignoring bower_components directory, in other words don't put bower_components
in .gitignore file. 

That's it, Actually with this method you can use whatever you want for your blog.