---
layout: post
title: Sending email through mailgun and wordpress
date: '2017-11-26 16:00:00'
tags:
- wordpress
- php
---

On digitalocean with the mailgun wordpress plugin, for some weird reason it is not working even though I configured [postfix](http://www.postfix.org/).

I'm following the tutorial already through setting up a relay with these tutorials: [How to Set Up a Mail Relay with Postfix and Mailgun on Ubuntu 16.04](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-mail-relay-with-postfix-and-mailgun-on-ubuntu-16-04)  and  [Configure Postfix to use Mailgun SMTP Relay on Ubuntu
](https://guides.wp-bullet.com/configure-postfix-use-mailgun-smtp-relay-ubuntu/).

After setting it up, I realized it still would not pickup from that. So, I decided to use the `mail()` of PHP. The reason is that if I call `wp_mail()` in another plugin, and I do not know yet if mailgun plugin has kicked in already (that's still something I should research).

So what happened was first try to use the default `mail()` function, then if it still fails (`$result = false`) then try `wp_mail()` (which I do not know if mailgun plugin already over-rode).

My next step to make it more elegant is to actually put Mailgun's latest class through composer and use [Bedrock](https://roots.io/bedrock/) so wordpress is using [composer](https://getcomposer.org/).
