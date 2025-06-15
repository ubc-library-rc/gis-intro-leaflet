---
layout: default
title: 3. Map Boilerplate 
parent: Hands On with Leaflet
nav_order: 3
---

# Map Boilerplate
A [boilerplate](https://www.freecodecamp.org/news/whats-boilerplate-and-why-do-we-use-it-let-s-check-out-the-coding-style-guide-ac2b6c814ee7/) is a chunk of code that can be used as-is in multiple contexts and often provides the basis for more advanced operations. The boilerplate code for this workshop renders a basemap which we will tinker with and add to in order to build an dynamic cluster map. It’s important that you don’t lose any of this code, and that it remains in its original structure and arrangement. Beyond this workshop, before you experiment with it on your own it's a good idea to make a copy of the original code to refer back to.


## Boilerplate Code
Now that we've seen what the boilerplate basemap for this workshop looks like, let’s explore the code behind it. Return to VS Code (your code editer). Double click `boilerplate.html ` in the Explorer panel to open it. The contents of your boilerplate should look like this: 


```html
<html>
  <head>
    <title>Leaflet Boilerplate</title>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Source for your Leaflet JavaScript and CSS -->
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
    integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
    crossorigin=""/>
     <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
      integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
      crossorigin=""></script>

    <script src="./ubcbuildings.js" charset="utf-8"></script>
  </head>

  <body>
    <!-- Your map's HTML container -->
    <div id="mapid" style="height: 100%;"></div>

    <!-- Script for your map between <script> and </script> -->
    <script>

      // Initialize your map, sets the initial view location and zoom level
      var mymap = L.map('mapid').setView([49.2827, -123.1207], 11);

      //Load the tile layer, paste in new tile layer of choice.
      var OpenStreetMap_BZH = L.tileLayer('https://tile.openstreetmap.bzh/br/{z}/{x}/{y}.png', {
      attribution: 'Map Tiles By <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, Tiles courtesy of <a href="http://www.openstreetmap.bzh/" target="_blank">Breton OpenStreetMap Team</a>',
      subdomains: 'abcd',
      minZoom: 0,
      maxZoom: 20,
      ext: 'png',
      scrollWheelZoom: false,
    }).addTo(mymap);

      //Paste your marker here

      //Paste the L.geoJSON function here

      //Paste popup function here

    </script>
  </body>
</html>

```



## Anatomy of an HTML document 
The HTML document is split into two main sections: the <code>head</code> and the <code>body</code>. Each of these sections are contained within opening < tags > and closing </ tags >. Notice that because the document is in HTML format, everything is contained within the html tag.

```html
<html>
  <head>
    The stuff inside the head is the metadata for your browser about the
    document. Inside the head are things like the document’s title - in this
    case “Boilerplate Code” - so that it can used for things like being
    displayed in your browser’s tab. Additionally, there are links to the source
    code for Leaflet's JavaScript and CSS rules. If you copy either one of those
    links and paste it in a new tab in your browser, you’ll see a lot of raw
    code. By linking to the source, we avoid having to carry this text into our
    own document, while also being assured that the code we’re using is
    up-to-date.
  </head>

  <body>
    The body contains what you see formatted in your browser. In the code above,
    the body contains directions for rendering and displaying an interactive
    map centered on Vancouver.

    <div>
      This element states how tall and how wide the map should be on the screen.
    </div>

    <script>
      Included in the body is a block of JavaScript that loads the map on the screen.
      Continue to the next section for a better understanding of this script...
    </script>
  </body>
</html>
```


---

## Some Notes

- **Version Releases** In the <head> element of your map's HTML document you will see links to Leaflet's CSS and Javascript responsible for the styling and interactivity of your boilerplate basemap. Notice both links include `leaflet@1.9.4`. This refers to the Leaflet version. Just as your computer occasionally requires software updates, Leaflet occasionally releases updates. If your web maps ever stop working for no apparent reason, go to Leaflet's home page, [leafletjs.com](https://leafletjs.com/) and check if a new version has been released. If it has, simply update your CSS and Javascript links to match. 
    

- **Linking Data Sources** Beneath the Leaflet CSS and Javascript is the line `<script src="./ubcbuildings.js" charset="utf-8"></script>`. This is a link to the map data, wrapped as a javascript variable. While this will be explained further in the following pages, it is important to note two things. First, always link your map data in the head of your map's HTML document. Second, the `./` preceding the filename denotes a relative path. A [relative path](https://www.w3schools.com/html/html_filepaths.asp) is a path to a file that is in the same folder as your HTML document. If your data were stored in downloads, for instance, the source link would look like `src="./downloads/ubcbuildings.js"`. If your data were stored on a server or hosted by an external web source, as are the CSS and Javascript, the source link would direct the web browser reading and rendering your map's HTML document to that address. 

