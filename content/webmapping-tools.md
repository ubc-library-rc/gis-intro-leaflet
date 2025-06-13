---
layout: default
title: Web Mapping Tools
parent: Introduction
has_children: true
nav_order: 3
---

Here, outline different tools, and link to demos nested as subpages (or links to our other workshops, in the case of mapbox and qgis2web plugin). show in workshop if there is interest, otherwise save as resources and focus workshop hands-on on teaching leaflet. 

# Tools for Web Mapping
{: .no_toc}
Describe range. And reasons for choosing one or the other. code. describe apis. edit the below descriptions, from spatial stories workshop, to be more tailored to this workshop and the audience. 

umap, mapbox, QGIS plugins, leaflet. today's workshop will use leaflet. code. why. 

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

We recommend Google Maps for its Google MyMaps service *only*. With Google MyMaps, you create simple maps with drop pin locations or imported data layers, like the below map: 
<iframe src="https://www.google.com/maps/d/embed?mid=13jisTC20ztRT93EJS0u_6u4_lzvEehk&ehbc=2E312F" width="640" height="480"></iframe>

While the Google Maps Platform offers a panoply of mapping tools including [dynamic maps](https://mapsplatform.google.com/maps-products/dynamic-maps/), you must be very careful about surreptitious charges. For example, while the [embed maps API](https://developers.google.com/maps/documentation/embed/get-started?hl=en) is free with unlimited usage, you must sign up for Google Cloud. Google Cloud is only free for 90 days then will charge you $200 monthly. In our opinion, it is recommended to invest your time and energy in learning a free and open-source option like uMap or Leaflet. 


----
## uMap
[uMap](https://umap.openstreetmap.fr/en/) is a free and open-source platform that allows you to create webmaps using OpenStreetMap (OSM) data. You can then embed these maps into a website, or simply share the link with collaborators and audiences. You can choose from a variety of basemaps, and even upload and add data layers of your own! uMap is very easy to use, but has little room for customization. It is an entirely web-based interface and requires no prior expertise. 

The below map was created in 5 minutes using data downloaded from Vancouver [open data portal](https://opendata.vancouver.ca/explore/dataset/parks-polygon-representation/information/). 


<iframe width="100%" height="500px" frameborder="0" allowfullscreen allow="geolocation" src="//umap.openstreetmap.fr/en/map/vancouver-parks_1219886?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#12/49.2605/-123.0997"></iframe><p><a href="//umap.openstreetmap.fr/en/map/vancouver-parks_1219886?scaleControl=false&miniMap=false&scrollWheelZoom=true&zoomControl=true&editMode=disabled&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=none&captionBar=false&captionMenus=true#12/49.2605/-123.0997">See full screen</a></p>

<!-- 
<iframe src="http://u.osmfr.org/m/1219886/" style="width:100%; height:500px"></iframe> -->
----

mapbox (both code side and not)

QGIS --> web plugin -- see workshop

storymaps alternative --> knightlab. throw in some information of making story including maps, such as storymaps and knightlab. to see more options and think through kinds of outputs if you arent sure, see spatial stories workshop resource. 

<br>


----

## Mapbox
[Mapbox](https://www.mapbox.com/) is a robust Geospatial **S**oftware **A**s **A** **S**ervice (saas) for developers, and includes products such as toolkits for mobile app development, navigation, web maps, and data management. Mapbox's service model is based on a paid subscription, but they offer a free service tier for those interested in using Mapbox products for learning. You will be asked to put in credit card information, however.  If this is your first time hearing about Mapbox, *[How Mapbox Works](https://docs.mapbox.com/help/getting-started/)* provides a great introduction.

> #### Mapbox Advantages  ⇡
> {: .no_toc}
> - Platform for custom styling basemaps
> - Variety of different services, including both code and web-based graphical user interface for web mapping

> #### Mapbox Disadvantages ⇣
> {: .no_toc}
> - Mapbox is proprietary, and the functions are not transposable between other webmapping libraries like Leaflet
> - The Free Tier has limitations that might be of concern to you if you intend to make a map that will be widely viewed and cited
> - Though you can make maps in Mapbox Studio, developing more custom webmaps requires working with code. Even then, Leaflet can often be more customizable because it is open-source and there is more code out there to draw from. 

#### Resources for working with Mapbox
{: .no_toc}
- UBC Research Commons' [Intro to webmapping with Mapbox](https://ubc-library-rc.github.io/intro-mapbox/) workshop
- [Intro to Mapbox studio](https://docs.mapbox.com/studio-manual/guides/)
- [Choropleth maps with Mapbox](https://labs.mapbox.com/education/thematic-map-types/choropleth/)
- [Heatmaps with Mapbox Studio](https://docs.mapbox.com/help/tutorials/studio-heatmap-tutorial/)
- [Dot Density maps with Mapbox](https://labs.mapbox.com/education/thematic-map-types/dot-density/)
- [Graduated Symbol maps with Mapbox](https://labs.mapbox.com/education/thematic-map-types/graduated-points/)


Below is an example of a cluster map made with mapbox:

<iframe src="./reference/mapbox-cluster-map.html" style="width:90%; height:400px; border:none; "></iframe>

----
## Leaflet
<img src="./images/leaflet_logo.png" alt="Leaflet Logo" style="margin: auto; width:35%" />

Leaflet is a set of instructions that your web browser or mobile device uses to display maps and let you interact with them. For example, when you double click your mouse on a map, leaflet tells your browser to zoom in. Leaflet defines the style of your map and includes things like zoom controls, attribution links, pop-ups, colors for markers and more. Leaflet is made up of only 38kb of Javascript, so it is really fast and lightweight - meaning browsers don’t have to work very hard to load it. Leaflet is open source, free, and hugely customizable. And, because of this, Leaflet is widely used. There are lots of alternatives to Leaflet, like for example Google Maps, which you need an API key to use.

<!-- ## Leaflet
[Leaflet](https://leafletjs.com/) consists of JavaScript and CSS code libraries which power the ways your web browser interprets and interacts with geospatial data & displays colors and style. For instance, when you double click a map to zoom in, Leaflet is at work. When you add data to your map, Leaflet assigns it a default color. Leaflet is made up of only 38kb of Javascript, so it is really fast and lightweight - meaning browsers don’t have to work very hard to load it.  -->

### As Code
Leaflet consists of JavaScript and CSS code libraries which power the ways your web browser interprets and interacts with geospatial data & displays colors and style. For instance, when you double click a map to zoom in, Leaflet is at work. When you add data to your map, Leaflet assigns it a default color. And because Leaflet is open-source, the code is hugely customizable and extensible. This means you can re-mix the code all you want — which you will do in this workshop. [Here are some examples](https://leafletjs.com/plugins.html) of Leaflet-based plugins to give you some idea of the variety of added functionality that comes from the community of developers.

### In a Browser
Take a look at this basic [Leaflet map example](./leaflet-example.html). You can zoom in, pan around, etc. It's meant to be displayed in your internet browser or a mobile application, so it loads and responds to you quickly.  



<iframe src="./leaflet-example.html" style="width:100%; height:500px; border:none;"> </iframe>


> #### Leaflet Advantages  ⇡
> {: .no_toc}
> - Leaflet is free and open source. For this reason, Leaflet is widely used. 
- As an open-source code library, Leaflet is hugely customizable. This means you can re-mix the code all you want. 
> - Leaflet is beginner friendly, though you do need to interact with code in order to build your map.
> - Hugely customizable. Leaflet-based plugins to give you some idea of the variety of added functionality that comes from the community of developers. 
> - In Leaflet, you can [change the CRS](https://leafletjs.com/reference.html#crs) of your map whereas the projection is set in Google Maps and Mapbox. 

> #### Leaflet Disadvantages ⇣
> {: .no_toc}
> - You'll need to work with code in a code editor. This can introduce a semi-steep learning curve, but you can truly create a basic webmap in a few hours with no prior knowledge. 
> - You'll need a place to store your map and map data. Github can work. Think about how you'll be displaying your end product. Will it be embedded on a website? 
<!--could do a tutorial thats like lets make a map and add data to github and make github page-->