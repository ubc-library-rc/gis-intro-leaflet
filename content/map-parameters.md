---
layout: default
title: 4. Map Parameters 
parent: Hands On
nav_order: 4
---

# Map Parameters: A closer look at the script
<br>
Everything you add to the boilerplate during this workshop will be within the script tags. Let's take a closer look at what's already there and modify each parameter to see how customizable even the basemap can be. 

```js
<script>
var mymap = L.map('mapid').setView([49.2827, -123.1207], 11);

var OpenStreetMap_BZH = L.tileLayer('https://tile.openstreetmap.bzh/br/{z}/{x}/{y}.png', {
      attribution: 'Map Tiles By <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, Tiles courtesy of <a href="http://www.openstreetmap.bzh/" target="_blank">Breton OpenStreetMap Team</a>',
      subdomains: 'abcd',
      minZoom: 0,
      maxZoom: 20,
      ext: 'png',
      scrollWheelZoom: false,
    }).addTo(mymap);
</script>
```
