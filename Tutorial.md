# Iceland in QGIS: A Supplemental Tutorial on Adding Layers
### Author: william.kingren@mavs.uta.edu
## This tutorial is designed so you can practice the skills you used in the [Programming Historian QGIS Tutorial](http://programminghistorian.org/lessons/qgis-layers) about adding layers.

---------

1. Make a folder or directory called "Iceland" on your computer.

2. Download the follwoing data sets from DIVA-GIS [Google "DIVA-GIS Countries"] into that directory and **unzip each downloaded folder** into the Iceland directory.
* Administrative Areas: ISL_adm.zip
* Roads: ISL_rds.zip

3. Open QGIS and set up a new project.

4. Set up CRS (Coordinate Reference System) so that the project is using the **ISN93/Lambert 1993** Projected Coordinate System.
* Go to **Project** in the menu bar
* Select **Project Properties** from the drop-down menu
* Select **CRS** from the side bar of the new window
* type **isn93** in the filter field, then select **ISN93/Lambert 1993**

5. Build a base map: Open the following vectors by selecting **Layer** **Add Layer** then **Add Vector Layer**. Change the way they look using **Properties** (either double click on the layer or right-click and select **Properties**. Under **Style** click on **Simple Fill**, go to **Colors**, **Fill**, **Transparent Fill**.
* ISL_adm0.shp; change so there is no color fill
     * Under **Style** click on **Simple Fill**
     * go to **Colors**
     * Select **Fill**
     * Select **Transparent Fill**
* ISL-adm1.shp; same as above
* ISL_roads.shp; go to **Style** to change the color and width of the lines so they are easier to see

6. Look at the attribute table of ISL_adm1.shp by right clicking on the layer and then clicking on **Open Attribute Table**. These show the country's 8 Regions. Note that table **Name_1** gives the name of the Region. Write down the name of that column and close the attribute table.
* Go into the **Properties** for ISL_adm.shp
* Select **Labels** from the side menu
* Select **Show Labels for this layer** from the drop-down menu
* Open next drop-down menu **Label with** and select the name of your column
* Increase the size of your font till it is clearly visible on the map (i.e. 18pt)

7. Go to Blackboard and from the Iceland tutorial area, download the file named Iceland_1849.zip. Unzip it into your Iceland directory and import the .tif file into QGIS as a raster file by clicking **Layer** **Add Layer** then ** Add Raster Layer**. Note: I have already geo-referenced this file.

8. In the **Layers Panel** drag the Iceland_1849 raaster layer to the bottom of the list so the Region and Names are superimposed on the map.

9. Go back to properties of ISL_adm0.shp and ISL_adm1.shp and in the style tab change the width of the lines so they are visible.

10. Unselect **Iceland_1849** in the **Layers Panel**

11. Go back to Blackboard and download the file named Iceland_1697.zip in your Iceland directory and **repeat steps 7 and 8.**

12. Observe the difference in cartographic accuracy between the 1697 and 1849 maps by toggling between the two layers in the **Layers Panel**

13. **Save Your Work** and close QGIS- your done!

