---
layout: default
title: 6. Add Data
parent: Hands On with Leaflet
nav_order: 6
---

# Add Data
Let's add some map features!


## Add a single marker
- add a lookout etc. this will be what we'll add an image to later. 

Leaflet gives us an easy way to add basic map features called **markers**, which represent point locations on the ground. More information about adding basic features to Leaflet can be found in the [Leaflet Quick Start Guide](https://leafletjs.com/examples/quick-start/). Let's add a marker over UBC campus.    

To Do
{: .label .label-green }
Add a Leaflet marker by copy/pasting the text below into the <code>body</code> of your HTML document.


```js
var ubccampus = L.marker([49.260605, -123.245995]).addTo(mymap).bindPopup("Hello World!");
```    
You should see something like this (click on the marker too!):    

![Map loads over the center of UBC with a marker!](map05.png "Map loads over the center of UBC with a marker!")


## Add a point layer 
- community gardens 

GeoJSON are often more complex data than markers or shapes. But they can be added to your map similarly: by creating a new variable holding the values for the GeoJSON feature(s).    

Let's add a GeoJSON that represents UBC Buildings. Luckily, UBCs Campus and Community Planning releases [their geodata](https://github.com/UBCGeodata) as GeoJSON with an open license. For this workshop, the buildings variable has been pre-assembled, and came with the .zip data you downloaded at the beginning of this workshop (the file <code>ubcbuildings.js</code>).

If you ever wanted to make a variable for another geoJSON, this is how:
1. Start with a geoJSON file.
2. Wrap it as a variable:
```js
var [nameofyourvariable] = [your geoJSON text]
```
3. Save this file with a JavaScript file <code>.js</code> extension.

To add the UBC buildings variable to our map, we'll need to include a Leaflet geoJSON layer so that our map loads this data when initialized:    


To Do
{: .label .label-green }
Add the buildings to your map by copy/pasting the object below into your HTML document, just below the Marker.   


```js
L.geoJSON(ubcbuildings).addTo(mymap);
```    

You should see something like this after you save and reload your browser:    


![Map loads over the center of UBC with a marker, and a data layer!](map04.png "Map loads over the center of UBC with a marker, and a data layer!")


## Add a polygon layer
- parks 
add polygons and style



