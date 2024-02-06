---
layout: default
title: Change Base Map
parent: Hands On
nav_order: 4
---

# Change Base Map

Suppose we want our data to stand out from the green base map more than it does now. One thing we can do is change the source of the map tiles to one that has a more appropriate style for our blue data. As mentioned earlier, there are several out of the box options to choose from with a variety of different styles. [This page lists a number of different map tile sources](https://leaflet-extras.github.io/leaflet-providers/preview/), and provides the text to paste into our map document for each one (minus the important <code>.addTo(mymap)</code> which needs to be inserted before the final semi-colon). **some of these sources require an access token or api-key, so you won't be able to use them unless you sign up for an account**. 

    
The boilerplate basemap works well for this workshop, but try playing around with different tile layers. 


To Do
{: .label .label-green }
Copy the text below and replace the existing map tile variable in your HTML document.


```js
var Stadia_StamenTonerLite = L.tileLayer('https://tiles.stadiamaps.com/tiles/stamen_toner_lite/{z}/{x}/{y}{r}.{ext}', {
	minZoom: 0,
	maxZoom: 20,
	attribution: '&copy; <a href="https://www.stadiamaps.com/" target="_blank">Stadia Maps</a> &copy; <a href="https://www.stamen.com/" target="_blank">Stamen Design</a> &copy; <a href="https://openmaptiles.org/" target="_blank">OpenMapTiles</a> &copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors',
	ext: 'png',
      scrollWheelZoom: false,
    }).addTo(mymap);
```    

If it all went as planned, you should see the new basemap rendered by your browser. 
