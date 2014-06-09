---
layout: post
title: "Mapping Moves data, Part I"
modified: 2014-06-04 13:32:08 -0700
category: [web mapping]
tags: [location, web mapping, moves app]
image:
  feature: 
  credit: 
  creditlink: 
comments: 
share: 
---

An approach on mapping activity from the Moves app

###Why I use the Moves app###

Why? After moving to a new city (Portland, Or) and spending a considerable effort exploring the seemingly endless venues/coffee shops/restraunts/bars/parks, I realized I didn't have a good record of where I've been. On top of that, I'm biking, walking, and running like never before, so why not track that too? Simply, I wanted a way to easily both log the places I've been and how I got there. I'm an android user and after testing several far-too-feature-packed options, I settled on Moves. 

####Perks of the Moves app####
* Simple and fanastic UI
* It uses the Foursquare API to easily log your place
* Detects the type of your movement (ie biking, running, walking) 
* And finally, it now has a native tool to [export](https://accounts.moves-app.com/signin/export) your data in several formats (JSON, CSV, KML, GPX and ICS)

Basically, Moves is a great location tracking app disguised as a fitness tracker. 

**Disclaimer:** In April, [Facebook bought the Moves app](http://techcrunch.com/2014/04/24/facebook-acquires-activity-tracking-app-moves/). Moves [does share your data with Facebook](http://www.theverge.com/2014/5/6/5688334/moves-app-will-share-user-data-with-facebook), so that's something to consider. If you're an Android user, Google [does this already](http://www.babble.com/tech/creepy-cool-google-location-history-mapping-your-every-move/).
{: .notice}


###Mapbox & Tilemill###

The combination of Tilemill and Mapbox is one of the easiest ways to style and display your spatial data on the web. Coincidently, [Garret Miller](https://twitter.com/heyitsgarrett) at [Mapbox](https://www.mapbox.com/) made a [really nice tutorial](https://www.mapbox.com/blog/mapping-moves/) on how to export your Moves data, style it in [Tilemill](https://www.mapbox.com/tilemill/) and add a basemap through [Mapbox](https://www.mapbox.com) and publish your map online. I've chosen the Tilemill/Mapbox method mostly because I love Mapbox but also because they provide a really handy [GPX to GeoJSON tool.](https://github.com/mapbox/togeojson)

###My Moves###

<iframe width='100%' height='500px' frameBorder='0' src='http://a.tiles.mapbox.com/v3/rcallihan.iedo4jhh/attribution,zoompan,zoomwheel,geocoder,share.html'></iframe>

###Adding a Legend in TileMill###
A map of this nature is pretty useless without a legend. 


###Next posts###

I really haven't done much here that wasn't already described in Garret Miller's [post](https://twitter.com/heyitsgarrett), but in the next couple of posts I plan to accomplish a few extra things:

* Map places locations
* Show some strategies for cleaning up the Moves Polyline data

