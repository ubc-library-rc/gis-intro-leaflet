---
layout: default
title: Google MyMaps demo
parent: Web Mapping Tools
nav_order: 1
---
## Google MyMaps Demo
<br>

1. Go to [Google MyMaps](https://www.google.com/maps/d/u/0/). Create and/or login to your Google Account. 
<br><br>

2.  Click CREATE A NEW MAP  
 <img src="./images/create-new-mymap.png" style="width:25%">
<br><br>

3. Once a new map has been created, your screen will look like this. 
 <img src="./images/google-mymap-view.png" style="width:100%">
<br><br>

4. The interface is quite intuitive. In the top left-hand corner, there is a white box. The first thing you may notice is that your map is currently Untitled. You can simply click to edit the title. 
 <img src="./images/mymap-interface1.png" style="width:35%">
<br><br>

5. Beneath the title is a grey bar with options to "Add Layer", "Share", or "Preview".  
 - **Add Layer** will add additional layers to your map. Note: they will all be empty until you upload data to them. 
 - **Share** allows you to set the sharing options of your map, and send it to others. If you haven't given your map a name and description, you will be prompted to do so before sharing. 
 - **Preview** will give you a glimpse of how your map will look to others. 
<img src="./images/mymap-interface2.png" style="width:35%">
<br><br>

6. Each layer of your map will initially be untitled. You can change the name any time. The check box indicates whether the layer is visible or invisible on the map upon initial load. You can edit or delete a layer by clicking the three dots beside it. Remember that layers are containers for data, and each layer is empty until you upload data to it.     
<img src="./images/mymap-interface3.png" style="width:35%">
<br><br>

7. Lets go ahead and **add data to the map**. Note you can upload limited file types. Let's upload the dataset of Vancouver public libraries inside the `webmapping-workshop` data folder. The file is called `vpl.csv`. The data was taken from [Vancouver Open Data Portal](https://opendata.vancouver.ca/explore/dataset/libraries/information/) and edited slightly to update library addresses. 
<br><br>
 <img src="./images/vpl-csv.png" style="width:100%">
<br><br>
 To upload this dataset to your Google MyMap, click <img src="./images/mymap-import.png" style="width:8%"> and browse to the file. 
<br><br>
 You will be prompted to indicate the columns Google MyMaps should use to locate each feature. If you scroll down, lon and lat should be auto-selected. Keep these and click continue. 
 <br><br>
 <img src="./images/mymap-geo1.png" style="width:55%">
<br><br>
 Next, you will be prompted to choose the field containing the names of each feature for labelling purposes. It's always good to explore your dataset *before* importing it into any map. We will use `NAME`. Then click Finish.
<br> <br>
 <img src="./images/mymap-geo2.png" style="width:55%">
<br><br>
 If you haven't made a name for the layer, it will automatically take on the name of your uploaded file. 
<br>
 <img src="./images/mymap-datapoints.png" style="width:95%">
<br><br>

8. Right now, the drop-pins representing libraries are uniformly styled. This means that each icon is same color, size, shape, etc. We can change the styling of a layer by clicking the paint-roller icon <img src="./images/mymaps-uniform-style-icon.png" style="width:15%">. You can change the styling by grouping places/datapoints in the following ways:

- **Uniform style** What we have now. All points are styled the same. 
- **Sequence of numbers** Data points are each assigned a number
- **Individual styles** Allows you to manually adjust the color and icon for each occurrence. After setting "Group places by" "Individual styles", simply over over any place and click the grey paint icon that appears to the right. 
- **Style by data column** Will assign a random color to occurrence of the column selected. For instance, if we style by the column `NAME`, because each library has a unique name, each drop-pin will become a distinct color. 
<br><br>
 <img src="./images/mymaps-byname.png" style="width:95%">
<br><br>
In all cases, labels can be set according to any column of your dataset, or set to "No labels". 
<br>
Furthermore, you can continue to edit the styling individual points/places even after they are styled by data column. For example,

- Click the the paint-roller icon beside a place<br>
 <img src="./images/mymaps-vpl1.png" style="width:30%">

- Change the color and icon of a place<br>
 <img src="./images/mymaps-vpl2.png" style="width:25%">

- Add an image to a popup<br>
 <img src="./images/mymaps-vpl3.png" style="width:30%">
<br><br>


Finally, you can choose different basemaps to highlight your data. <br>
 <img src="./images/mymap-interface4.png" style="width:35%">