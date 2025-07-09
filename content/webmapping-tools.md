---
layout: default
title: Web Mapping Tools
has_children: true
nav_order: 2
---
# Tools for Web Mapping
{: .no_toc}
There are a variety of tools for making web maps. Some require you engage with code, while others provide simple drag-and-drop interfaces. In this workshop, you will learn how code works to power a web map, and be guided through customizing some given code, called "boilerplate code", to make a map of your own. However, it's helpful to know about some alternatives that don't require any coding! Outlined below are different tools/platforms for web mapping. Each option is evaluated for its relative affordances and limitations, and resources for continued learning are listed.

If, after this workshop, you are unsure whether web mapping itself best suits your project goals, check out our [spatial stories workshop](https://ubc-library-rc.github.io/gis-spatial-stories/) to see other output format options. You can also email `library.gis@ubc.ca` with questions, or book a 1:1 consult with the geospatial team [here](https://libcal.library.ubc.ca/appointments/research_commons#s-lc-public-pt).
{: .note}

<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>
----



## Google MyMaps 

We recommend Google as a web mapping platform for its *Google MyMaps service  only*. With [Google MyMaps](https://www.google.com/maps/about/mymaps/), you can create simple maps with drop pin locations or import data layers. Here's an example: 
<iframe src="https://www.google.com/maps/d/embed?mid=13jisTC20ztRT93EJS0u_6u4_lzvEehk&ehbc=2E312F" width="100%" height="480"></iframe>
<br>

#### Google Advantages and Disadvantages
{: .no_toc}
 - While the Google Maps platform offers a panoply of mapping tools including [dynamic maps](https://mapsplatform.google.com/maps-products/dynamic-maps/), you must *be very careful about surreptitious charges*. For example, while the [embed maps API](https://developers.google.com/maps/documentation/embed/get-started?hl=en) is free with unlimited usage, you must sign up for Google Cloud to use it. Google Cloud is only free for 90 days, after which you will be charged $200 monthly. In our opinion, beyond the simple drag-and-drop visualizations offered by Google MyMaps, it is recommended to invest your time and energy in learning a free and open-source option like uMap or Leaflet (detailed below). 
 - Very easy to make a map quickly; beginner friendly; no coding required
 - Limited customization 

#### Resources for Google MyMaps
{: .no_toc}
 - For a brief demonstration on setting up a web map with Google MyMaps, see the nested subpage, [MyMaps demo](./mymaps.md). 

----

## uMap
[uMap](https://umap.openstreetmap.fr/en/) is a free and open-source platform that allows you to create web maps using OpenStreetMap (OSM) data. You can then embed these maps into an existing website, or simply share the link to your final map with collaborators and audiences. With uMap, you can choose from a variety of basemaps, and even upload and add data layers of your own! uMap is very easy to use, and has ample customization options. It is an entirely web-based interface and requires no coding or prior expertise. 

The below map was created in 5 minutes using data downloaded from Vancouver [open data portal](https://opendata.vancouver.ca/explore/dataset/parks-polygon-representation/information/). 


<iframe width="100%" height="500px" frameborder="0" allowfullscreen allow="geolocation" src="//umap.openstreetmap.fr/en/map/vancouver-parks_1219886?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#12/49.2605/-123.0997"></iframe><p><a href="//umap.openstreetmap.fr/en/map/vancouver-parks_1219886?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#12/49.2605/-123.0997">See full screen</a></p>

<!-- 
<iframe src="http://u.osmfr.org/m/1219886/" style="width:100%; height:500px"></iframe> -->

#### Resources for uMap
{: .no_toc}
- For a demonstration on setting up a web map with uMap, see the nested subpage, [uMap demo](./umap.md). 

----

## QGIS to Web Map plugin 

If you’re familiar with [QGIS](https://qgis.org/), there’s actually a nifty plugin for turning your QGIS map into an interactive web map, either powered by Leaflet or OpenLayers. This plugin is aptly called [qgis2web](https://plugins.qgis.org/plugins/qgis2web/). Below is an example map created by the workshop author for the BC Disaster Resilience Research Network:

 <iframe src="https://lilydemet.github.io/island-mapping/" style="width:100%; height:600px;"></iframe>


#### qgs2web Advantages and Disadvantages
{: .no_toc}
- If you are somewhat familiar with QGIS, qgis2web is a super beginner-friendly way to make a web map. Especially if you aren't sure whether a web map is the right format for your project output, qgis2web is a great way to quickly visualize what your project might look like as a web map. 
- A disadvantage is you will need somewhere to store your map and map data, such as Github or a local server.
 

#### Resources for qgis2web
{: .no_toc}
- See the Research Common's [workshop on QGIS Plugins](https://ubc-library-rc.github.io/gis-plugins-qgis/content/webmapping.html) for a guided tutorial on how to not only make a webmap using the qgis2web plugin, but also host it online using Github.

----

## ArcGIS Online
[ArcGIS Online](https://www.arcgis.com/index.html) or (AGOL) is Esri's online platform for making dynamic and interactive maps. If you are a UBC faculty or student, you can learn more about obtaining access [here](https://gis.ubc.ca/software/#:~:text=FOR%20STUDENT%20PERSONAL%20COMPUTERS&text=This%20%2420%20license%20includes%20ArcGIS,reduced%20cost%20is%20also%20available.&text=This%20is%20a%20non%2Drefundable,installed%20on%20personal%20computers%20only.).

<iframe src='https://www.arcgis.com/apps/instant/basic/index.html?appid=23193586bdc34314a976d475e2cb867e' width="100%" height="500" style="border:none;"> </iframe>


#### ArcGIS Online Advantages  ⇡
{: .no_toc}
  - Allows you to load and save data online, as well as create dynamic maps with customizable basemaps, popups, and interaction

#### ArcGIS Online Disadvantages ⇣
{: .no_toc}
  - ArcGIS Online is proprietary, meaning it is not free to use
  - Licensing is a hassle, and collaboration can only occur between people who both own an active license

#### AGOL Resources
{: .no_toc}
 - Check out the Research Common's [workshop on ArcGIS Online](https://ubc-library-rc.github.io/gis-storymaps/) for more. 

----

## Felt
[Felt](https://felt.com/) is a web-based platform for creating aesthetic, interactive maps and dashboards with your data. They offer a free tier that allows you to make and share unlimited webmaps, as well as automatic 14-day free trial of middle tier. 
Checkout their [gallary](https://felt.com/gallery) to get inspired by their [examples](https://felt.com/map/Baltimore-City-Proposed-Land-Use-April-2024-DEElrNXBRICZ3XTKtmCYKD?loc=39.34342,-76.63756,13.9z). 


----

## Mapbox
[Mapbox](https://www.mapbox.com/) is a robust Geospatial **S**oftware **A**s **A** **S**ervice (saas) for developers, and includes products such as toolkits for mobile app development, navigation, web maps, and data management. Mapbox's service model is based on a paid subscription, but they offer a free service tier for those interested in using Mapbox products for learning. Below is an example of a cluster map made with mapbox:

<!-- mention mapbox (both code side and not). mention api.  -->

<iframe src="./reference/mapbox-cluster-map.html" style="width:90%; height:400px; border:none; "></iframe>

#### Mapbox Advantages  ⇡
{: .no_toc}
 - Platform for custom styling basemaps
 - Variety of different services, including both code and web-based graphical user interface for web mapping

#### Mapbox Disadvantages ⇣
{: .no_toc}
 - Mapbox is proprietary, and the functions are not transposable between other webmapping libraries like Leaflet
 - The Free Tier has limitations that might be of concern to you if you intend to make a map that will be widely viewed and cited
 - Though you can make maps in Mapbox Studio, developing more custom webmaps requires working with code. Even then, Leaflet can often be more customizable because it is open-source and there is more code out there to draw from. 

#### Resources for working with Mapbox
{: .no_toc}
 - If this is your first time hearing about Mapbox, *[How Mapbox Works](https://docs.mapbox.com/help/getting-started/)* provides a great introduction.
 - UBC Research Commons' [Intro to webmapping with Mapbox](https://ubc-library-rc.github.io/intro-mapbox/) workshop
 - [Intro to Mapbox studio](https://docs.mapbox.com/studio-manual/guides/)
 - [Choropleth maps with Mapbox](https://labs.mapbox.com/education/thematic-map-types/choropleth/)
 - [Heatmaps with Mapbox Studio](https://docs.mapbox.com/help/tutorials/studio-heatmap-tutorial/)
 - [Dot Density maps with Mapbox](https://labs.mapbox.com/education/thematic-map-types/dot-density/)
 - [Graduated Symbol maps with Mapbox](https://labs.mapbox.com/education/thematic-map-types/graduated-points/)




----

## Leaflet
<img src="./images/leaflet_logo.png" alt="Leaflet Logo" style="margin: auto; width:35%" />

[Leaflet](https://leafletjs.com/) is a set of instructions that your web browser or mobile device uses to display maps and let you interact with them. For example, when you double click your mouse on a map, leaflet tells your browser to zoom in. Leaflet defines the style of your map and includes things like zoom controls, attribution links, pop-ups, colors for markers and more. Leaflet is made up of only 38kb of Javascript, so it is really fast and lightweight - meaning browsers don’t have to work very hard to load it. Leaflet is open source, free, and hugely customizable. And, because of this, Leaflet is widely used. There are lots of alternatives to Leaflet, but most require an API key to use.


### As Code
{: .no_toc}

Leaflet consists of JavaScript and CSS code libraries which power the ways your web browser interprets and interacts with geospatial data & displays colors and style. For instance, when you double click a map to zoom in, Leaflet is at work. When you add data to your map, Leaflet assigns it a default color. And because Leaflet is open-source, the code is hugely customizable and extensible. This means you can re-mix the code all you want — which you will do in this workshop. [Here are some examples](https://leafletjs.com/plugins.html) of Leaflet-based plugins to give you some idea of the variety of added functionality that comes from the community of developers.

### In a Browser
{: .no_toc}

Take a look at this basic [Leaflet map example](./leaflet-example.html). You can zoom in, pan around, etc. It's meant to be displayed in your internet browser or a mobile application, so it loads and responds to you quickly.  



<iframe src="./parks-map.html" style="width:100%; height:520px; border:none;"> </iframe>


#### Leaflet Advantages  ⇡
{: .no_toc}
 - Leaflet is free and open-source. For this reason, Leaflet is widely used. 
 - As an open-source code library, Leaflet is hugely customizable. This means you can re-mix the code all you want. 
 - Leaflet is beginner friendly, though you do need to interact with code in order to build your map.
 - Hugely customizable. Leaflet-based plugins to give you some idea of the variety of added functionality that comes from the community of developers. 
 <!-- - In Leaflet, you can [change the CRS](https://leafletjs.com/reference.html#crs) of your map whereas the projection is set in Google Maps and Mapbox.  -->

#### Leaflet Disadvantages ⇣
{: .no_toc}
 - You'll need to work with code in a code editor. This can introduce a semi-steep learning curve, but you can truly create a basic webmap in a few hours with no prior knowledge. 
 - You'll need a place to store your map and map data. Github can work. Think about how you'll be displaying your end product. Will it be embedded on a website? 
<!--could do a tutorial thats like lets make a map and add data to github and make github page-->

----

## Options for Narrative Mapping
Finally, if you are looking to make more of a multi-media narrative, either including different kinds of maps or a string of multimedia displayed over a single web map, we recommend [ArcGIS Storymaps](https://storymaps.arcgis.com/) or [KnightLab StoryMaps](https://storymap.knightlab.com/). Check out the Research Common's workshop on [Creating StoryMaps with ArcGIS Online](https://ubc-library-rc.github.io/gis-storymaps/) for an introduction to making StoryMaps with the free version. Knightlab StoryMap offers a free and open-source product to visualize spatial stories. If you're not sure which of these tools is for you, we've detailed further explanation [here](https://ubc-library-rc.github.io/gis-spatial-stories/content/resources-narrative-mapping.html) under Assembling Resources in our [Spatial Stories](https://ubc-library-rc.github.io/gis-spatial-stories/) workshop. 