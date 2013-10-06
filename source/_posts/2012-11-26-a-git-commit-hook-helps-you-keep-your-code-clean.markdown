---
layout: post
title: "A git commit hook helps you keep your code clean"
date: 2012-11-26 22:18
comments: true
categories: [git, Drupal Planet, drupal]
---
I like to keep my code free of trailing whitespace. I feel what xjm describes as "[spinach in your teeth](http://xjm.drupalgardens.com/review-guide)" about whitespace and non-conforming coding standards.

I got (heavily) inspired by Josh The Geek's [git pre-commit hook](http://drupal.org/sandbox/JoshTheGeek/1143338), and made myself a commit hook that will check the code I am about to commit for common errors. In addition to whitespace, I like to make sure that I don't accidentally commit debug code like `krumo()`. The commit hook also checks for common calls to debug functions.

If you want to use it, simply put it in your .git/hooks folder in your git checkout. Make sure the file is executable with `chmod +x .git/hooks/pre-commit`. This will only effect the git checkout you put the commit hook in, but you can make it apply to all future checkouts by putting it in your git install directory's template folder. Where that folder is will vary, but on my mac it is in /usr/share/git-core/templates/hooks.

The script is not the most clever in the world, so it will be wrong about some things from time to time. You can override it and still commit with the command `git commit -n`

Here is the pre-commit file:
{% gist 4150599 %}
