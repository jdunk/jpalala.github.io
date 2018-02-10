---
layout: post
title: make npm3 install look like npm2
date: '2016-03-08 10:01:58'
---

Got this tip from a friend - [rico sta. cruz](http://ricostacruz.com/):

Just set the config to use `loglevel http` and not show the progress bar `progress false` and you're good to go.

`npm config set loglevel http && npm config set progress false`
