![Flag_of_Iceland.svg](/Flag_of_Iceland.svg.png)


# Iceland in QGIS: A Supplemental Tutorial on Adding Layers
### Author: william.kingren@mavs.uta.edu, with additions from Justin Jolly and Ahmed Foggie
## This tutorial is designed so you can practice the skills you used in the [Programming Historian QGIS Tutorial](http://programminghistorian.org/lessons/qgis-layers) about adding layers.

---------

1. Make a folder or directory called "Iceland" on your computer. *When working in QGIS, it is important to always save all files for a project in the same folder/directory.*

2. Download the Iceland data set from [DIVA-GIS](http://www.diva-gis.org) into that directory. In the drop down menu box labeled country, select Iceland. In the next drop down menu box labeled Subject, find the following data sets: 
* Administrative Areas: ISL_adm.zip
* Roads: ISL_rds.zip
**unzip each downloaded folder** into the Iceland directory.

3. Open QGIS and set up a new project.

4. Set up CRS (Coordinate Reference System) so that the project is using the **ISN93/Lambert 1993** Projected Coordinate System.
	* Go to **Project** in the menu bar
	* Select **Project Properties** from the drop-down menu
	* Select **CRS** from the side bar of the new window
	* type **isn93** in the filter field, then select **ISN93/Lambert 1993**

![Iceland Screenshot](/Iceland Screenshot.png)

5. Build a base map: Open the following vectors by selecting **Layer**, then **Add Layer**, then **Add Vector Layer**. Change the way they look using **Properties** (either double click on the layer or right-click and select **Properties**). Under **Style** click on **Simple Fill**, go to **Colors**, **Fill**, **Transparent Fill**.
* ISL_adm0.shp; change so there is no color fill.
     * Under **Style** click on **Simple Fill**
     * go to **Colors**
     * Select **Fill**
     * Select **Transparent Fill**
     
![Iceland Screenshot 2](/Iceland Screenshot 2.png)

* ISL-adm1.shp; same as above
* ISL_roads.shp; go to **Style** to change the color and width of the lines so they are easier to see.
* Keep these steps in mind. Later on, after you've geo-referenced your maps, you can re-enter the properties for your various layers and change them, which may help you glean useful information from your maps.

6. This is a good place to save your work!

7. Look at the attribute table of ISL_adm1.shp by right clicking on the layer and then clicking on **Open Attribute Table**. These show the country's 8 Regions. Note that table **Name_1** gives the name of the Region. Write down the name of that column and close the attribute table.
* Go into the **Properties** for ISL_adm1.shp
* Select **Labels** from the side menu
* Select **Show Labels for this layer** from the drop-down menu
* Open next drop-down menu **Label with** and select the name of your column: **Name_1**
* Increase the size of your font so that the labels are clearly visible on the map; an example size would be 18 pt., but it may depend on the size of your screen.

![Iceland Screenshot 3](/Iceland Screenshot 3.png)

8. Go to Blackboard and from the Iceland tutorial area, download the file named Iceland_1849.zip. Unzip it into your Iceland directory (where you have been saving all of your other files for this project) and import the .tif file into QGIS as a raster file by clicking **Layer**, then **Add Layer**, then ** Add Raster Layer**. Note: I have already geo-referenced this file.

9. In the **Layers Panel** drag the Iceland_1849 raster layer to the bottom of the list so the Region and Names are superimposed on the map.

10. Go back to properties of ISL_adm0.shp and ISL_adm1.shp and in the style tab change the width of the lines so they are visible.

11. Unselect **Iceland_1849** in the **Layers Panel**

12. Go back to Blackboard and download the file named Iceland_1697.zip in your Iceland directory and **repeat steps 7 and 8.**

13. Observe the difference in cartographic accuracy between the 1697 and 1849 maps by toggling between the two layers in the **Layers Panel**.
* The 1849 map should look more accurate when observing the outer regions. 

14. **Save Your Work** and close QGIS - you're done!

