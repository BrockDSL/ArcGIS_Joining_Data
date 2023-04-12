![image showing connection between values and map features](https://user-images.githubusercontent.com/45638590/228618024-2f77ded9-2227-4edf-a1d8-dcb041b2d6ba.png)

# Joining Tabular Data to Geospatial Data
This tutorial will look at the steps necessary for joining tabular data to geospatial data using ArcGIS Pro and ArcGIS Online.

----

## Setup Instructions
In preparation for this tutorial, you will need an organizational account with Esri. If you are a Brock user, you will sign into the software using your Brock credentials.

Data files:  
[TreeSampleChippawaCOORDINATES.xlsx](TreeSampleChippawaCOORDINATES.xlsx)    
[TreeSampleChippawaATTRIBUTES.xlsx](TreeSampleChippawaATTRIBUTES.xlsx)  

**The Scenario**  
We will be mapping tree sample data for the neighbourhood of Bridgewater near Niagara Falls and Chippawa. Tree data is often collected with GPS units that capture Geographic Coordinates. Unlike the previous exercise that required street addresses, this activity will plot the X,Y data then join detailed attributes. Sometimes it is easier to collaborate on a field project by having one person record the attributes such as diameter at breat height, tree species, health while another person captures the GPS coordinates. Although this example uses point data, the same general steps would apply to boundary files such as census tracts or municipal boundaries and associated tabular data.


----

## Displaying X,Y Data in ArcGIS Pro  

Open the Excel files to see the tabular data before beginning this tutorial. Notice that each table includes an OBJECTID field. First we will display the X,Y data found in TreeSampleChippawaCOORDINATES.xlsx and then the attribute data will be joined with the geospatial data using ArcGIS technologies.

Screenshot of the COORDINATE data:  
![image of coordinate data](https://user-images.githubusercontent.com/45638590/228039559-18895ed2-14fd-47e2-b9d9-0b8a4676e4fe.png)  

Screenshot of the ATTRIBUTE data:  
  ![image of tabular data](https://user-images.githubusercontent.com/45638590/228039769-3812e7da-155e-4340-a88a-d9e786392436.png)   

1. Run ArcGIS Pro and sign in to Your ArcGIS Organization's URL **brock.maps.arcgis.com** > Brock University (authenticate using Brock credentials)    
2. From the **Map** tab, click ![image of Add Data button](https://user-images.githubusercontent.com/45638590/228562697-56d115fa-a1ec-4ea1-8c21-76374c9f84f2.png)
3. Add the .xlsx worksheet that includes coordinate details. If prompted to update drivers, try saving the xlsx file as a comma separated values (CSV) file. The table appears under **Standalone tables**.  
  
   ![image of standalone tables](https://user-images.githubusercontent.com/45638590/231500314-33fd32b5-ed95-4a95-b4ce-822978d78f24.png)

4. Right click the table and select **Display X,Y data**  ![image of display xy data](https://user-images.githubusercontent.com/45638590/228290643-a6387503-9083-4bdd-98e1-fc8bb5fb5892.png)
5. Confirm that the X coordinate is matched to Longitude and the Y coordinate is matched to Latitude.  

**NOTE: The default coordinate system works for our data but you will need to be sure the coordinates you are using match the appropriate coordinate system. Contact [maplib@brocku.ca](mailto:maplib@brocku.ca) for assistance.**  

  ![image of Display XY data dialogue box](https://user-images.githubusercontent.com/45638590/231500864-0bcfec1c-5e82-4f85-8f12-dd87d86bcf85.png)

Here is a screenshot of the result:  

  ![image of map showing dots](https://user-images.githubusercontent.com/45638590/231501229-17efdc1e-ab40-4d64-96f7-cd92a16703b2.png)

  
## Joining in ArcGIS Pro

1. From the **Map** tab, click ![image of Add Data button](https://user-images.githubusercontent.com/45638590/228563080-aa5cc71a-5151-457a-b147-1b2b926e697a.png). 
2. Add the **tabular data** from the Excel worksheet called "TreeSampleChippawaATTRIBUTES > Sheet1$". Alternately, add a CSV version of the spreadsheet.
   
   ![image showing content listing with attribute CSV](https://user-images.githubusercontent.com/45638590/231501745-df653014-f914-4d3f-ab46-17d8d40369bf.png)

   
3. From the Contents list, right click the point feature layer and select **Joins & Relates > Add Join**  
4. Read each entry carefully to match the OBJECTID field for each data set. See image below:  
   
   ![image of Add join window](https://user-images.githubusercontent.com/45638590/231502658-864c8376-a3e1-4d27-a7f6-fb27e8fbc4fc.png)
   
5. Click OK to run the tool.  
6. Open the attribute table for the point feature layer and scroll across (if necessary) to see the newly joined attributes.  
   
   ![image of attribute table with join](https://user-images.githubusercontent.com/45638590/231503043-2a719fc9-49fe-4011-8ac4-5b578beca3a9.png)


## Displaying in ArcGIS Online  

1. Go to https://arcgis.com and sign in to your ArcGIS Organization using your Brock University credentials.  
   
   ![image of your arcgis organization's URL](https://user-images.githubusercontent.com/45638590/228044683-49c2251a-2630-4b20-9f32-de4082156383.png)  
   
2. Click the **Map** tab at the top of the screen.  
3. Click **Add > Add layer from file**  
4. Click **YOUR DEVICE** and browse to the file ![image of name and file type CSV](https://user-images.githubusercontent.com/45638590/231506073-59fbc519-f26a-49c6-bf95-b5778ef52733.png) 
   
5. Accept the defaults for the *Fields*, click **Next**.  
6. Under **Location** settings, select **Latitude and Longitude** from the dropdown options.  
7. Match the fields accordingly.  
8. Click Next.  
9. Enter a *Title, Folder location in ArcGIS Online, Tags and Summary*.  
10. Click **Create and add to map**.  
   
   ![image of ArcGIS online with map of points](https://user-images.githubusercontent.com/45638590/231505793-e2f54694-62ca-40e3-9df3-ac65348eb808.png)  
   
11. To add the tabular attribute data, click **Add > Add layer from file**.  
12. Click **YOUR DEVICE** and browse to the file ![image of attribute CSV](https://user-images.githubusercontent.com/45638590/231506710-b816e52d-c66e-41e3-93bb-a2d6cefc9ce6.png)

14. Click Next.
15. Accept all the fields to add and click **Next**.
16. From the **Location** settings, choose ![image showing selection option](https://user-images.githubusercontent.com/45638590/228048791-4efbdc14-f218-4ad7-834b-eddd918af270.png)
17. Click Next.
18. Enter a *Title, Folder, Tags and summary*.  
19. Click **Create and add to map**. 
20. In ArcGIS Online, the tables can be found by clicking the table icon ![image of tables icon](https://user-images.githubusercontent.com/45638590/228049393-b11dcbcd-b5fb-4cfe-92a8-f6360c17cd93.png) from the left menu options.  
21. Before continuing, click the layers icon ![image of layers icon](https://user-images.githubusercontent.com/45638590/228049947-7c305f23-e993-47ec-966a-4ec466e95e22.png)
 


## Joining in ArcGIS Online

1. With the point feature layer active (it will have a blue bar down the side), click the analysis tools from the righthand menu ![image of analysis tools icon](https://user-images.githubusercontent.com/45638590/228050174-f94a9178-95ad-4448-b75d-3d7a581f0d67.png)
2. Click the hammer icon ![image of hammer icon](https://user-images.githubusercontent.com/45638590/228323895-9741b872-54ea-4811-be1e-8509f6ef9c32.png)
3. From the list of geoprocessing tools, under **Summarize Data**, select **Join Features**. 
4. Select the point feature layer as the **Target** Layer.  
5. Select the table as the **Join** Layer.
6. Scroll down to **Join Settings**.
7. Select OBJECTID for both the Target layer and the Join layer.
   
   ![image of Join Settings dialogue box](https://user-images.githubusercontent.com/45638590/228324823-14643566-2a2d-4c8d-a913-7115d0485a08.png)
   
8. Scroll down to the **Result Layer** section and enter a unique output name. 
   
9. Click **Run**.
10. To see the status of the tool, click the **History** button ![image of history icon](https://user-images.githubusercontent.com/45638590/228325510-58538221-a5aa-4f75-b8b9-a5c987de4992.png).  
11. The resulting feature layer will automatically be added to the map. Click a dot to see the attribute listing in a pop-up. 

**NOTE: you may need to turn off visibility of the original point layer.**

![image of popup illustrating join result](https://user-images.githubusercontent.com/45638590/231508546-a0f0fce9-1d5d-40f6-bb0c-6fbb075e6f04.png)

More information about Joins & Relates can be found [here](https://pro.arcgis.com/en/pro-app/latest/help/data/tables/joins-and-relates.htm).  

----

## Next Steps (Optional)
[Visualizing geospatial data](https://brockdsl.github.io/ArcGIS_Visualization/)

----

**This tutorial is supported by the Brock University Research Lifecycle Department; Map, Data & GIS Library.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [maplib@brocku.ca](mailto:maplib@brocku.ca)**
