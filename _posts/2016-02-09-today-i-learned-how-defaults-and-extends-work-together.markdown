---
layout: post
title: 'today i learned how _.defaults and _.extends work together'
date: '2016-02-09 06:44:32'
---

So today I just discovered the `_.extends` function of underscore. There's a little known function that is similar, called `_.extendsOwn`. This basically is the underscore version for the upcoming 'Object.assign' method of ES6.

I didn't like how javascript mutates objects and doesn't make the code any easier to understand. So in a function I was creating that originally mutates to object without returning anything, I needed a way to copy the object and modify it, then return it back. One way to do that is to get copy the object to another variable, completely and without reference to the original object that got passed in. So that's what led me to figure out how to use [extend](http://underscorejs.org/#extend) and decided on using [extendOwn](http://underscorejs.org/#extendOwn)

Long story cut short - I wanted more info about these functions which led me to this article:

[Extending objects in underscore](https://lostechies.com/chrismissal/2012/10/05/extending-objects-in-underscore/)

There's this method that is very similar to extend, called `_.defaults` that is really useful. Imagine you have an existing object that you dont want certain properties (and their values) to be overwritten when merging other objects into it. That's what defaults are for basically. Any present values in the existing object wont get overwritten by other object's attributes.

The use cases are for the times that you want to exclude certain properties when merging together objects.  One application is pushing data to an incrementing indexing NoSQL database that absolutely must have the same **identifier** in the JSON message, to be able to search for it later. 

So cool. For more info on extend, checkout this [2ality article](http://www.2ality.com/2012/08/underscore-extend.html)
