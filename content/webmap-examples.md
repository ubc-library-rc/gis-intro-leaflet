---
layout: default
title: Reference vs Thematic
parent: Introduction
nav_order: 3
---
# Kinds of Web Maps
Explain. reference vs thematic. 
While this workshop will focus on reference webmaps, resources for xyz will be noted/linked below.

## Reference Webmaps
The most basic reference webmap is simply a basemap, contained in a viewbox with controls and an attribution at the bottom. Much like their static counterparts, reference webmaps can be as simple as a basemap with a drop-pin locator or a single data layer. Explore the interactive capabilities of each of the following examples.

<iframe src="./reference/jawg-map.html" style="width:90%; height:450px; border:none;"> </iframe>
<br>
<iframe src="./reference/leaflet-reference-map.html" style="width:90%; height:450px; border:none;"> </iframe>
<br>
<iframe src="https://www.google.com/maps/d/embed?mid=13jisTC20ztRT93EJS0u_6u4_lzvEehk&ehbc=2E312F" width="640" height="480"></iframe>


<iframe width="100%" height="500px" frameborder="0" allowfullscreen allow="geolocation" src="//umap.openstreetmap.fr/en/map/vancouver-parks_1219886?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#12/49.2605/-123.0997"></iframe><p><a href="//umap.openstreetmap.fr/en/map/vancouver-parks_1219886?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#12/49.2605/-123.0997">See full screen</a></p>

<!-- 
now show one with a simple data layer - like parks
*Maybe add an example that's like: a nice walk I took.*

other reference maps > weather underground, open street maps- google maps, osmAnd. show one also thats made from qgis to web.  -->

### Some popular reference webmaps out there:
<iframe src="https://native-land.ca/" width="640" height="640"></iframe>

<iframe src="https://www.queeringthemap.com/" width="640" height="640"></iframe>


---- 


## Thematic Webmaps 
Thematic web maps visualize the results of some spatial analysis. With a bit of code, you can create choropleth, cluster, and proportional symbol web maps.

<sub>[See below choropleth example as full-page map](./reference/leaflet-choropleth-map.html)</sub>
<iframe src="./reference/leaflet-choropleth-map.html" style="width:90%; height:400px; border:none;"> </iframe>

  
<sub>[See below cluster map example as full-page map](./reference/leaflet-cluster-map.html)</sub>
<iframe src="./reference/leaflet-cluster-map.html" style="width:90%; height:450px; border:none;"> </iframe>
    
<sub>[See below cluster map example as full-page map](./reference/mapbox-cluster-map.html)</sub>
<iframe src="./reference/mapbox-cluster-map.html" style="width:90%; height:400px; border:none; "></iframe>


<sub>[See below proportional symbol map example as full-page map](./reference/leaflet-proportional-symbol-map.html)</sub><br> Hover over the circles to learn the municipality population for Vancouver Island.
<iframe src="./reference/leaflet-proportional-symbol-map.html" style="width:90%; height:450px; border:none; "></iframe>


(must discuss later - these often require processing data in software first, like qgis -- could do an advanced workshop on that) also include little note for each indicating what tools software or workflows used to make it. (see mychestnut tree link elswhere) 

(also discuss making reference or thematic more elaborate in leaflet, with timesliders etc)