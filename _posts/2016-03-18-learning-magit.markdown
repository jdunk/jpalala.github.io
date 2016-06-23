---
layout: post
title: Learning magit
date: '2016-03-18 11:02:36'
---

I attended a recent Javascript meetup where [Zak](https://twitter.com/zakame) showed us the power of using [emacs](https://www.gnu.org/software/emacs/) for javascript.

For me, other than note taking, the thing I like to really learn is using the emacs [magit plugin](https://www.emacswiki.org/emacs/Magit). To get it installed in a cinch, I did `brew install magit`. Yes, I am lazy and [brew](http://brew.sh/) is amazing. Also note that I also got the emacs from brew as well, btw.

One thing I struggled a bit was intalling other plugins. After getting the [melpa](http://ergoemacs.org/emacs/emacs_package_system.html) repo wired in to emacs, it was a simple `M-x list-packages` and then `Ctrl-s magit` (which searches for magit) then pressing i (mark install) and x (execute).

So for my first thing to try, I went to my dotfiles repo and tried to commit something new. After opening a file using `$ emacs <filename>`, I just typed `M-x magit-` and pressed TAB. I found the command to use: `M-x magit-commit` and then typed my commit message. Then, to finish up the commit and actually commit, I typed `C-c C-c`. And it was commited. 

Since I was on master and will push to master, I just did `M-x magit-push-popup` and then pressed P. 

Well magit was  easier than I thought it was. Hope it was a nice introduction to using magit. 

I'm pretty sure I'm just touching the tip of the iceberg of what it can do, will keep posting new learnings about using magit as I go along.

 
[^1]: Note: C = Ctrl key. Learn more - https://www.emacswiki.org/emacs/EmacsKeyNotation