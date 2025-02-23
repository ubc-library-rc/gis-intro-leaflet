---
layout: default
title: Practice
nav_order: 4
---
# Practice
Practice what you've learned in this workshop by choosing a dataset from Vancouver’s [open data portal](https://opendata.vancouver.ca/explore/?disjunctive.features&disjunctive.theme&disjunctive.keyword&disjunctive.data-owner&disjunctive.data-team&sort=modified) to add to your webmap. You will need to download the dataset in GeoJSON format, move it to your `intro-leaflet-data` folder, wrap it as a javascript variable, and add as both a a data source and a data layer to your html document. 

Note: You may need to change your map centering and zoom level so Vancouver comes into the frame. 

Take a moment to practice on your own, or refer to the hints below. 

1. For example, download [Vancouver Parks](https://opendata.vancouver.ca/explore/dataset/parks-polygon-representation/export/) (polygon representation) from the Open Data Portal. 
<img src="./vanparks-opendataportal_20240827.png" style="width:100%;">

2. Move the download file, `parks-polygon-representation.geojson` to your workshop folder, `intro-leaflet-data`. It's important your data be in the same folder of your webmap's html document. 
    

3. Open the dataset in VS Code. It will either appear in your Contents after you add it to your working folder, or you can right-click it from your computer and open it with VS Code. 
    

4. It will look like a wall of code. Right-click anywhere on the page and format it. 
<img src="./format-document_20240827.png" style="width:100%;">
    

5. Now wrap it as the variable `vanparks`
<img src="./var-vanparks-geojson_20240827.png" style="width:100%;">
    

6. You'll notice the name of the document becomes red, signifying there's a syntax error somehwere in the document. There isn't. Rather, you have formatted the document as javascript, but the file extension is still GeoJSON. Save your work (hit Ctrl + S) and return to your `intro-leaflet-data` on your computer. Rename the file  Rename the file and file extension: `vanparks.js`. 
<img src="./rename-file_20240827.png" style="width:30%;">

7. Return to VS Code and open the new dataset, `vanparks.js`. Everything should be in order now with no warnings. 


8. Now, return to your `boilerplate.html` document in VS Code. In the `<head>` tag, add a line beneath your current data source that directs your map to your new data source: 
```
<script src="./vanparks.js" charset="utf-8"></script>
```

9. Then, in the `<script>` tag of the body element, add a function to add your second data source as a layer: 
```
L.geoJSON(vanparks).addTo(mymap);
```

10. Save your html file and go to your Live Server. Zoom out and pan to Vancouver. You should see your data layer added to the map. 

<img src="./webmap-with-data_20240827.png" style="width:100%;">



--- 

# Next Steps

If this workshop has inspired you to expand your skills, try making another map on your own using data for a different location on your own. This will give you some clarity around where you might have some gaps in understanding. Remember, you can create your own GeoJSON with free tools like [geojson.io](http://geojson.io).

***Keep in mind that not all data will be nicely packaged and cleaned. In fact, it never is. If you proceed to use data that you've found on the web, be prepared to spend time preparing your data to be usable with Leaflet and the web.***

### More Resources for Web Mapping
This workshop builds from several other resources for web mapping. Here are some great places to start extending your knowledge:

Web map basics: [Anatomy of a Web Map - Alan McConchie and Beth Schechter](http://maptime.io/anatomy-of-a-web-map/)    
Leaflet basics: [Leaflet Quick Start Guide](https://leafletjs.com/examples/quick-start/)   
Web map functionality examples: [Mapbox.js Examples](https://docs.mapbox.com/mapbox.js/example/v1.0.0/)    
GeoJSON: [More than you ever wanted to know about GeoJSON - Tom MacWright](https://macwright.org/2015/03/23/geojson-second-bite.html)    
    

<!--
### License
[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
-->
