---
layout: default
title: Examples
parent: Introduction
nav_order: 3
---
# Different kinds of web maps... 
Maps can be static or dynamic, they can be digital, web-based, or physical, and often, projects will incorporate more than one kind of map in their output. However, any map can be categorized into one of two main kinds of maps: **reference maps** and **thematic maps**. 

Reference maps are useful to show the lay of the land, such as the geographic context surrounding your research location or area of interest. Reference maps can be as simple as a drop pin location, or more complex with data layers, labeling, and insets. Thematic maps, on the other hand, use visualization techniques such as color, size, shape, and density to convey further information about a dataset. Writes Statistics Canada: “A thematic map shows the spatial distribution of one or more specific data themes for standard geographic areas.” For example, a map showing the population of each neighborhood by a color gradient would be a thematic map, as it visualizes the spatial distribution of population within the geographic area of a neighborhood. 

There is a case to be made that all maps are thematic, as the definition of boundaries, borders, names, etc. is a political and almost always contested act. In other words, there are no neutral maps that simply represent an objective reality or truth. See [Crampton and Krygier (2006)](https://acme-journal.org/index.php/acme/article/view/723) for a seminal introduction to critical cartography, or [Wang and Liu (2022)](https://www.researchgate.net/publication/365011390_Maps_and_cartography_Progress_in_international_critical_cartographyGIS_research) for an overview of critical cartography and GIS through the last several decades. See also *The Power of Maps* by Denis Wood. 

This workshop will focus on the anatomy and construction of reference web maps. However, examples of both reference web maps and thematic web maps are included below. Take a moment to familiarize yourself with what these may look like. The next section will introduce the different tools and platforms with which they were made. 
 
----


## Reference Web Maps
The most basic reference web map is simply a basemap, contained in a viewbox with controls and an attribution at the bottom. Much like their static counterparts, reference web maps can be as simple as a basemap with a drop-pin locator or a single data layer. Explore the interactive capabilities of each of the following examples.

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

### Some other reference web maps out there:

- [Falling Fruit](https://fallingfruit.org/locations/embed?z=10&y=49.24090&x=-483.04568&m=true&t=roadmap&c=forager,freegan&l=false&locale=en) is a foraging map, hosted by Google Maps. Everyday people can anonomysouly upload finds such as a lush patch of blackberries, alleyway lemonbalm, or a plum tree in a yard slated for demolition. 

- [Native-land.ca](https://native-land.ca/) shows Indigenous territories across Turtle Island and around the world. You can search First Nations by territories, languages, or treaties. The map can be overlaid upon a colonial, cartesian basemap. This web map is powered by Mapbox, with basemap tiles from Open Street Map. 

- [Queering the map](https://www.queeringthemap.com/) visualizes anonymized, user-submitted queer experiences around the world. While their basemap used to be Google Maps, it recently changed to Open Street Map. It's unclear what library is powering the interactivity of this web map, but extended documentation is impressively available on [Radical-data's Github](https://github.com/radical-data/queering-the-map). 




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

The construction of thematic web maps often requires prior data processing and modification in software such as QGIS. 

<!--  could do an advanced workshop on that) also include little note for each indicating what tools software or workflows used to make it. (see mychestnut tree link elswhere) -->


<!-- (also discuss making reference or thematic more elaborate in leaflet, with timesliders etc) -->