---
layout: post
title: 
date: '2016-08-26 01:30:59'
tags:
- first-post
---

### 

Hello Singapore! It was a pleasure to visit this place. Here's what I did.

8/21
====

Arrival at SG. Met my cousin and hanged out at a KFC in Changi Airport. Their chicken salad was fresh and had lots of chicken. 

We then went out of Changi Airport through the Skytrain, to the real MRT. We dropped off at Tanah Merah. From there, we took the green line straight to Buono Vista, the station nearest my hotel. 

8/22
====

PHPConf had a Tutorial Day over at AWS office in Capital Square.

I learned a lot about docker and am currently still obsessing over it.

I realized I'm missing out a lot then, and heard of something called [Caddy Server with PHP for docker](https://hub.docker.com/r/abiosoft/caddy/)

You can get it by just running `docker run -d -p 2015:2015 abiosoft/caddy`.Just set the path bellow to your php code, and you'll have it running in localhost:2015 (read more from the [README.md](https://github.com/abiosoft/caddy-docker#php)

`$ docker run -d -v /path/to/php/src:/srv -p 2015:2015 abiosoft/caddy:php`

8/23
====

The first day of the conference. Looking up Matrix Biopolis was hard on the map, but you just go a road that goes on a hill and it will be on your left.

So I learned quite a lot especially the one on Web Security, how to become a great developer (tests, talk, and keep improving). Davey Shafik ([@dshafik](https://twitter.com/dshafik)) talked about PHP still being quite popular, running on about 80% of servers. It is dying in the sense of people not quite switching over to version 7, but that's because it's still pretty raw. Let's make it ripe by helping out! 

In the evening, I checked out the Sommerset area, and ate at Four Fingers. I wish I bought that electronic gadget at a mac store there, it's just a keyboard, but it's by microsoft called the Arc. Dang.

8/24
===
This day went by a breeze. I woke up late and checked out some things first on Laravel Ph community. I attended the talks and some topics were interesting, including Migrating to PHP7, where Paul Dragoonis ([@dr4goonis](https://twitter.com/dr4goonis)) talked about using two piplines to push into. I enjoyed checking out the new stuff with Microsoft Azure, particularly Nano Server. I learned a lot from the DBA guy Harald Zeitlhofer ([@HZeitlhofer](https://twitter.com/HZeitlhofer)), he talked about learning about SQL caching and how to optimize queries instead of relying on the codebase to do the ORM work for you.

Another thing was meeting Ms April Kwong ([@araphoenix](https://twitter.com/araphoenix)) who hails from the Philippines and works now with Function8 (https://www.facebook.com/functioneightltd). She's looking for Laravel developers by the way in the Philippines. She talked about Laravel and its many features which make it awesome.

The drupal talk was alright, not touching core is one of their tennets, and it was enjoyable. Even more fun was the Machine Learning thing. Didn't know PHP could do that, but yeah it's all about using an https://secure.php.net/manual/en/book.fann.php. 

The last talk was a bit long but unfortunately I had to go (had a flight at 7ish), so grabbed my bag and though I felt really bad, I was gonna miss the after-party, it was OK. Maybe that's something to look forward to in the next SG PHP conf :) 
