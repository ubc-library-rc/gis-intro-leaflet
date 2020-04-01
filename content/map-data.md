---
layout: default
title: Data
parent: Basic Components
nav_order: 3
---

# Map Data
Another moving part of a web map is the data added to it. While your map tiles are a necessary part of your map, they're really only there to provide reference to your data. Your data sits on top of your basemap. We call this your "data layer", "map content" and sometimes your "map features". Most of the time, your data is vector data so you can click and interact with it, but you can also add raster data as well.      

If you're a GIS user, you have encountered a Shapefile. Shapefiles are the industry standard file type for geographic vector data. If you've ever tried to share a Shapefile in the web, you've probably had some problems or the needed to transform your file into something else. Shapefiles are meant to be used in GIS and other software and weren't designed to be displayed in the web. [GeoJSON](https://geojson.org/) on the other hand, are geographic files which are meant for the web. They're "easy for humans to read, and easy for machines to read", meaning that they're a lightweight, simplified and format so your average web browser can use them, and they're also fairly easy to understand if you want to view and edit them in a code editor. Here's a GeoJSON point over UBC:

```json
    {
      "type": "Feature",
      "properties": {
        "name": "The University of British Columbia"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          -123.25012207031249,
          49.26186749272789
        ]
      }
    }
```
In contrast, a Shapefile is a binary (not text) format, so you wouldn't be able to read the file with human eyes. For these reasons, we're using GeoJSON files for this workshop.

One other great thing about GeoJSON, is that becuase they are open-source and simple to understand, there are several tools that allow you to create and edit them in the web, like [geojson.io](http://geojson.io).

To Do
{: .label .label-green }
1. Copy the GeoJSON text above and paste it in the </>JSON panel in [geojson.io](http://geojson.io).
2. Click the edit layer button (above the trash can) to move the marker to a different position, then save.
3. In the Table panel, edit the GeoJSON file's attributes, by changing the name of the location.
