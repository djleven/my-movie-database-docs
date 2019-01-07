---
id: 119
title: Shortcode default parameters
date: 2017-10-21T00:24:03+00:00
layout: post
guid: 127.0.0.1/?p=119
permalink: /shortcode-default-parameters/
---
As is mentioned in the documentation, the default values for the shortcodes are:

id=655 and type=movie

So this means that when you want to display a movie you don&#8217;t need to set the type parameter.

The default values for rest of the available shortcode parameters are taken from whatever is selected in your &#8216;my-movie-database&#8217; option page settings. In other words you should set these parameters only if you wish to override the &#8216;global&#8217; plugin settings. We&#8221;ll look at these again later.

Now why would anyone put in a default id? 

Basically, the default id is set is for demonstration purposes. I figured if you do not enter an id, it&#8217;s then better to get something back instead of some ugly warning message.

The choice of 655 corresponds to an a old favourite tvshow of mine Star Trek TNG. When I saw the 655 id for a movie happens to correspond to &#8220;Paris Texas&#8221; (which I have yet to see but that&#8217;s beside the point), then the &#8216;quality assurance&#8217; test was passed, and 655 became default.

So then, if you post the shortcode tag with the &#8216;tvshow&#8217; type parameter, but do not include your choice of id, then you will get Star Trek TNG.

So [my\_movie\_db type=tvshow] returns:

{% include TMDB/StarTrekTNG.html %}

Now if you simply post the shortcode tag without any parameters at all you will get the movie  &#8220;Paris Texas&#8221; which shares the same id,  but is a movie (type).

So [my\_movie\_db] will get you :

{% include TMDB/ParisTexas.html %}

##### Realistic Scenarios

Of course in all the realistic scenarios you will have to set the id yourself. We&#8217;ll look at some more examples next.