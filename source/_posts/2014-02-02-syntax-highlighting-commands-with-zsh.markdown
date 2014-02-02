---
layout: post
title: "Syntax highlighting commands with Zsh"
date: 2014-02-02 13:48:19 +0100
comments: true
categories: [cli, zsh, oh-my-zsh, syntax-color, terminal]
---
I started using zsh about a year ago after having resisted it with a passion.
My main worry was that I would "forget how to bash" and be lost on various servers I log in to. While there are some nifty things I have gotten a little too used to in zsh, I don't think it has been a big problem.

One thing that visually tells me that I am in zsh and not bash is that my zsh terminal syntax highlights as I type. Yes, you read that correctly. If you are not familiar with the [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) prepare to have your mind blown.

When you are typing a command you get a yellow color:

{% img https://dl.dropboxusercontent.com/u/157691/cdn/naxocnet/zsh/zsh-syntax-1.png %}


Then when you have typed something that actually is a command you get green:

{% img https://dl.dropboxusercontent.com/u/157691/cdn/naxocnet/zsh/zsh-syntax-2.png %}


When you make a typo you get red:

{% img https://dl.dropboxusercontent.com/u/157691/cdn/naxocnet/zsh/zsh-syntax-3.png %}


It also makes correctly quoted strings yellow. I find that a nice help too:

{% img https://dl.dropboxusercontent.com/u/157691/cdn/naxocnet/zsh/zsh-syntax-4.png %}

On the [Github project](https://github.com/zsh-users/zsh-syntax-highlighting) readme there are instructions for installing the plugin.
