---
title: DroneDeploy
weight: 1
---

# DroneDeploy

**Creating a project**

[Video Tutorial](https://youtu.be/e0vZLDi6CIs)

1. Navigate to the relevant folder. If one doesn't exist for the state that your flight(s) is/are located in, then create one.
2. Click on the create project icon ![](RackMultipart20230818-1-nllyam_html_a054b1eb7c956865.png) .
3. Navigate to the general location of your project and click on the 'Create Project Here' icon.
4. Name your project and select the 'Standard' model.

![](RackMultipart20230818-1-nllyam_html_583b22bf2dbcb4f5.png)

1. This is where you will set up your autonomous flight(s).
2. Rename your flight by clicking on the three dots next to Map Plan.
3. To add multiple flights to a project, simply click on the blue plus sign ![](RackMultipart20230818-1-nllyam_html_aaf92a698f75ad02.png) located next the Map Plan name. You can then access each flight by using the drop down.

![](RackMultipart20230818-1-nllyam_html_67a7b7ef453e1bd8.png)

**Setting up autonomous flights**

1. Delineate your valley bottom(s) for the extents of desired flights.
  1. These shapefiles must have a CRS of WGS84 (EPSG:4326)
2. Import your valley bottom shapefile(s) to the relevant [DroneDeploy](https://dronedeploy.com/) project using the Import KML or SHP app.

![](RackMultipart20230818-1-nllyam_html_d93c348690dbdea1.png)

1. Adjust the flight plan settings as necessary.
  1. Altitude
  2. 3D enhancement
  3. Flight direction
  4. Obstacle avoidance

**Make flight plans available offline**

1. On the iPad mini, open up DroneDeploy.
  1. The interface is the same as on the web browser.
2. While connected to the internet, navigate to your project.
  1. The projects you created on the web browser should sync automatically.
3. Select the plan you want to make available offline.
4. Turn off Automatic Settings
5. Select the toggle for 'Make Available Offline'
6. Allow plan to fully sync before closing the app.
7. Before heading into the field, make sure that your plan is downloaded for offline use.
  1. Turn on airplane mode
  2. Close the app
  3. Re-open the app and ensure its available and displaying properly.
  4. You can also restart the iPad and repeat steps above.

![](RackMultipart20230818-1-nllyam_html_592f4170e910e273.png)

**Uploading imagery to Box and DroneDeploy (Post-Flights)**

[Video Tutorial](https://youtu.be/Dx-pgS56O6g)

1. Create a folder on Box to house all of your drone data.
  1. This folder should be named after the month and year that the imagery was captured (i.e. June\_2023)
  2. Within the 'Month\_Year' folder you should create separate folders for each flight that was captured in the field.
  3. Within those folders you should create the following folders:
    1. Elevation: _houses the elevation models from DroneDeploy_
    2. Geomorphic\_Mapping: _houses the mapping that is done later on_
    3. Obliques: _houses the oblique imagery that was captured in the field_
    4. Orthoimagery: _houses the high-res orthoimage from DroneDeploy_
    5. Raw: _houses the individual images from the field prior to mosaicking_

![](RackMultipart20230818-1-nllyam_html_a647fade85abcc42.png)

1. Delete ground photos.
  1. Prior to takeoff, the drone always takes a photo of the ground. Go through and delete these photos from the SD card.
2. For each flight, move the oblique photos from the SD into the relevant 'Oblique' folders.
3. For each flight, move the raw photos from the SD into the relevant 'Raw' folders.
4. In DroneDeploy, navigate to the relevant project and press the 'Upload' tab at the top of the screen.

![](RackMultipart20230818-1-nllyam_html_d7132628d05a63d1.png)

1. Drag and drop your photos from the 'Raw' folder into the upload pane.
  1. After the upload is complete, the images need to be processed by DroneDeploy before the products will be available for export. This can take a few hours.

**Exporting DroneDeploy products**

1. Once the processing has been completed, you can access the available data by clicking the 'Explore' tab and navigating to the date that the images were collected.

![](RackMultipart20230818-1-nllyam_html_311db12037b754ef.png)

1. From there, click the 'Export' icon at the bottom left of the screen

![](RackMultipart20230818-1-nllyam_html_d1fb9ce3dbe3e221.png)

1. Select the product you want to export
  1. The two products we will almost always export are the GeoTIFF Mapp (which is the orthoimage) and the DTM.

![](RackMultipart20230818-1-nllyam_html_58481e9c5f8bce38.png)

1. Exporting the Orthoimagery
  1. Select the GeoTIFF option
  2. Change the email address from Wally's email to yours
  3. Make sure the file type is GeoTIFF
  4. Change the resolution to 2 in/px
  5. Click 'Export'

![](RackMultipart20230818-1-nllyam_html_d7179efd595037.png)

1. Exporting the DTM
  1. Select the DTM option
  2. Change the email address to your email
  3. **Make sure file type is** **Raw Elevation Values (DTM)**
  4. Click 'Export'

![](RackMultipart20230818-1-nllyam_html_9afcefba73c8d274.png)

1. Once you select 'Export' the products will begin processing. Once the processing is complete you will receive an email from drone deploy with a link to download the product. Save each product into their designated folders on Box
  1. Orthoimage goes to the Orthoimagery folder
  2. DTM goes to the Elevation folder

**Other Resources**

DroneDeploys documentation on flight planning

[**https://help.dronedeploy.com/hc/en-us/articles/1500004964302-Mobile-App-Flight-Planning**](https://help.dronedeploy.com/hc/en-us/articles/1500004964302-Mobile-App-Flight-Planning)

DroneDeploys documentation on exporting data

[**https://help.dronedeploy.com/hc/en-us/articles/1500004964642-Exporting-Your-Data**](https://help.dronedeploy.com/hc/en-us/articles/1500004964642-Exporting-Your-Data)