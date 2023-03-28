Add in the tutorial image here 

![Tool Logo](Image filename)

# Joining Tabular Data to Geospatial Data
This tutorial will look at the steps necessary for joining tabular data to geospatial data using ArcGIS Pro and ArcGIS Online.

----

## Setup Instructions
In preparation for this tutorial, you will need an organizational account with Esri. If you are a Brock user, you will sign into the software using your Brock credentials.

data files: 
TreeSampleChippewa_COORDINATES.xlsx  
TreeSampleChippewa_ATTRIBUTES.xlsx

**The Scenario**  
We will be mapping tree sample data for the neighbourhood of Bridgewater near Niagara Falls and Chippewa. Tree data is often collected with GPS units that capture Geographic Coordinates. Unlike the previous exercise that required street addresses, this activity will plot the X,Y data then join detailed attributes. Sometimes it is easier to collaborate on a field project by having one person record the attributes such as diameter at breat height, tree species, health while another person captures the GPS coordinates. Although this example uses point data, the same steps would apply to boundary files such as census tracts or municipal boundaries and associated tabular data.


----

## Displaying X,Y Data ArcGIS Pro  

Open the Excel files to see the tabular data before beginning this tutorial. Notice that each table includes an OBJECTID field. First we will display the X,Y data found in TreeSampleChippewa_COORDINATES.xlsx and then the attribute data will be joined with the geospatial data using ArcGIS technologies.

Screenshot of the COORDINATE data:  
![image](https://user-images.githubusercontent.com/45638590/228039559-18895ed2-14fd-47e2-b9d9-0b8a4676e4fe.png)  

Screenshot of the ATTRIBUTE data:  
![image](https://user-images.githubusercontent.com/45638590/228039769-3812e7da-155e-4340-a88a-d9e786392436.png)   


1. Run ArcGIS Pro and sign in to Your ArcGIS Organization's URL **brock.maps.arcgis.com** > Brock University (authenticate using Brock credentials)    
2. Add the .xlsx worksheet for location information 

![image](https://user-images.githubusercontent.com/45638590/228290539-56173057-9be4-4d49-a60a-c15f2c124b61.png)
  
  
4. Right click the table and select **Display X,Y data**  ![image](https://user-images.githubusercontent.com/45638590/228290643-a6387503-9083-4bdd-98e1-fc8bb5fb5892.png)
5. Confirm that the X coordinate is matched to Longitude and the Y coordinate is matched to Latitude.  

**NOTE: The default coordinate system works for our data but you will need to be sure the coordinates you are using match the appropriate coordinate system. Contact maplib@brocku.ca for assistance.**  

![image](https://user-images.githubusercontent.com/45638590/228290825-e2037d19-2c7d-4965-88c6-fa9176b31645.png)
  
Here is a screenshot of the result:  

![image](https://user-images.githubusercontent.com/45638590/228291294-e393b4a1-8b36-4fba-a530-6b3730dea4a7.png)
  
## Joining in ArcGIS Pro

1. Add the attribute worksheet called "TreeSampleChippewaATTRIBUTES > Sheet1$"  

![image](https://user-images.githubusercontent.com/45638590/228292987-37223506-4167-43ef-b775-83eefa3b7dae.png)
 
2. From the Contents list, right click the point feature layer and select **Joins & Relates > Add Join**  
3. Read each entry carefully to match the OBJECTID field for each data set. See image below:  

![image](https://user-images.githubusercontent.com/45638590/228293750-97efdf3a-cd70-473a-bacd-997cb96db77a.png)

4. Click OK to run the tool.
5. Open the attribute table for the point feature layer and scroll across (if necessary) to see the newly joined attributes.  

![image](https://user-images.githubusercontent.com/45638590/228294207-81ea8544-3203-44e3-a9cb-112c84e1f262.png)




## Displaying in ArcGIS Online  

1. Go to https://arcgis.com and sign in to your ArcGIS Organization using your Brock University credentials  

![image](https://user-images.githubusercontent.com/45638590/228044683-49c2251a-2630-4b20-9f32-de4082156383.png)  

2. Click the Map tab at the top of the screen.
3. Click Add > Add layer from file
4. Click YOUR DEVICE and browse to the file ![image](https://user-images.githubusercontent.com/45638590/228046076-8499935e-d128-44bb-9d72-69453ceb71ea.png)
   
5. Accept the defaults for the field to include, click Next.  
6. Under Location settings, select **Latitude and Longitude** from the dropdown options.
7. Match the fields accordingly.  
8. Click Next.
9. Enter a Title, Folder location in ArcGIS Online, Tags and Summary.
10. Click **Create and add to map**.

![image](https://user-images.githubusercontent.com/45638590/228048193-6438eeb8-fc67-4cc8-b54a-4de4e3aa9ed1.png)  

11. To add the tabular attribute data, click Add > Add layer from file
12. Click YOUR DEVICE and browse to the file ![image](https://user-images.githubusercontent.com/45638590/228045678-9e9f9454-4e43-45e7-83df-bdca7fc76197.png)  
15. Click Next.
16. Accept all the fields to add and click Next.
17. From the location settings, choose ![image](https://user-images.githubusercontent.com/45638590/228048791-4efbdc14-f218-4ad7-834b-eddd918af270.png)
18. Click Next
19. Enter a Title, Folder, Tags and summary.  
20. Click Create and add to map. 
21. In ArcGIS Online, the tables can be found by clicking the table icon ![image](https://user-images.githubusercontent.com/45638590/228049393-b11dcbcd-b5fb-4cfe-92a8-f6360c17cd93.png)
 from the left menu options.  
22. Before continuing, click the layers icon ![image](https://user-images.githubusercontent.com/45638590/228049947-7c305f23-e993-47ec-966a-4ec466e95e22.png)
 


## Joining in ArcGIS Online

1. With the point feature layer active (it will have a blue bar down the side), click the analysis tools from the righthand menu ![image](https://user-images.githubusercontent.com/45638590/228050174-f94a9178-95ad-4448-b75d-3d7a581f0d67.png)


  
  
 

----

## Next Steps (Optional)
This is where you can add any additional resources, follow up tutorial, or workshop reccomendations that users might use to continue learning about the tool described in the tutorial.  The more the better!

----

**End notes**
This is where you mention the DSL, MDGL, or Research Lifecycle department and put in contact information.  An example of what this might look like is:

**This tutorial is supported by the Brock University Research Lifecycle Department.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [DSL@Brocku.ca](mailto:DSL@Brocku.ca)**
