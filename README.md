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






Each tutorial will be different based on the tools used.  Breaking the tutorial up into individual steps is highly reccomended as it reduces congnitive load and allows for "break points" where users can stop and start from at their leisure.  Each step should cover no more than 1 or two concepts and should always assume that the user has minimal experience (explain every action in as granular detail as possible).

If you are enhancing your tutorial with embedded content like H5P modules or Youtube videos, make sure to check how they will look on different mediums.  Generally they will look good on any computer monitor or projector but depending on where you got the embed code from it may not adjust nicely for mobile and tablet viewing.

When embedding an iframe, make sure to place at least 2 blank lines above and below it in the markdown file to avoid the HTML interfereing with your markdown syntax.

----

## Next Steps (Optional)
This is where you can add any additional resources, follow up tutorial, or workshop reccomendations that users might use to continue learning about the tool described in the tutorial.  The more the better!

----

**End notes**
This is where you mention the DSL, MDGL, or Research Lifecycle department and put in contact information.  An example of what this might look like is:

**This tutorial is supported by the Brock University Research Lifecycle Department.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [DSL@Brocku.ca](mailto:DSL@Brocku.ca)**
