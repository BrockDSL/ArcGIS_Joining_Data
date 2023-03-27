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

## Displaying X,Y Data 

Open the Excel files to see the tabular data before beginning this tutorial. Notice that each table includes an OBJECTID field. First we will display the X,Y data found in TreeSampleChippewa_COORDINATES.xlsx and then the attribute data will be joined with the geospatial data using ArcGIS technologies.

Screenshot of the COORDINATE data:
![image](https://user-images.githubusercontent.com/45638590/228039559-18895ed2-14fd-47e2-b9d9-0b8a4676e4fe.png)  

Screenshot of the ATTRIBUTE data:
![image](https://user-images.githubusercontent.com/45638590/228039769-3812e7da-155e-4340-a88a-d9e786392436.png)   


Run ArcGIS Pro and sign in to Your ArcGIS Organization j

add the xlsx worksheet called 
right click the table and select Display X,Y data
select GCS coordinate system

insert image of x,y data

## Joining in ArcGIS Pro

add the attribute worksheet called "

right click the point feature layer and select JOINS & RELATES > Join

OBJECTID field common to each table

insert image

click Run.

open the attribute table for the point feature layer.


## Joining in ArcGIS Online  

Go to https://arcgis.com and sign in to your ArcGIS Organization using your Brock credentials




----

## Next Steps (Optional)
This is where you can add any additional resources, follow up tutorial, or workshop reccomendations that users might use to continue learning about the tool described in the tutorial.  The more the better!

----

**End notes**
This is where you mention the DSL, MDGL, or Research Lifecycle department and put in contact information.  An example of what this might look like is:

**This tutorial is supported by the Brock University Research Lifecycle Department.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [DSL@Brocku.ca](mailto:DSL@Brocku.ca)**
