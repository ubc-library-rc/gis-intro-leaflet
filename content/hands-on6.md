---
layout: default
title: 6. Add Data
parent: Hands On with Leaflet
nav_order: 6
---

# Add Data
Let's add some map features! In this section, you will be shown how to add a single marker, a point data layer, and a polygon layer. You will also be shown how to change their styling. 

## Add a single marker
Let's add a marker for a nice resting spot with a lookout. Once done, you are encouraged to add a second marker in the same way that locates another spot you like in the city. If you happen to have an image of it, keep that close as we'll add it to a popup later. 

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





- **Linking Data Sources** Beneath the Leaflet CSS and Javascript is the line `<script src="./ubcbuildings.js" charset="utf-8"></script>`. This is a link to the map data, wrapped as a javascript variable. While this will be explained further in the following pages, it is important to note two things. First, always link your map data in the head of your map's HTML document. Second, the `./` preceding the filename denotes a relative path. A [relative path](https://www.w3schools.com/html/html_filepaths.asp) is a path to a file that is in the same folder as your HTML document. If your data were stored in downloads, for instance, the source link would look like `src="./downloads/ubcbuildings.js"`. If your data were stored on a server or hosted by an external web source, as are the CSS and Javascript, the source link would direct the web browser reading and rendering your map's HTML document to that address. 


Additionally, as we will see in the next step. adding data as we will see in the next step, is not as simple as adding geojson. Rather, we will "wrap a geosjson file as a variable and save as javascript file"  then link that file in the head of our leaflet map html document.
{: .note}    