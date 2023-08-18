---
title: DroneDeploy
weight: 1
---

## Creating a project
***

[Video Tutorial](https://youtu.be/e0vZLDi6CIs)

1. Navigate to the relevant folder. If one doesn't exist for the state that your flight(s) is/are located in, then create one.
2. Click on the create project icon <img src="{{ site.baseurl }}/assets/images/Project_Icon.png" width="300">.
3. Navigate to the general location of your project and click on the 'Create Project Here' icon.
4. Name your project and select the 'Standard' model.
5. This is where you will set up your autonomous flight(s).
6. Rename your flight by clicking on the three dots next to Map Plan.
7. To add multiple flights to a project, simply click on the blue plus sign ![](RackMultipart20230818-1-nllyam_html_aaf92a698f75ad02.png) located next the Map Plan name. You can then access each flight by using the drop down.



## Setting up autonomous flights
***

1. Delineate your valley bottom(s) for the extents of desired flights. **_Note: these shapefiles need to have a CRS of WGS84 (EPSG:4326)_**

2. Import your valley bottom shapefile(s) to the relevant [DroneDeploy](https://dronedeploy.com/) project using the Import KML or SHP app.

3. Adjust the flight plan settings as necessary.
    - Altitude
    - 3D enhancement
    - Flight direction
    - Obstacle avoidance

## Make flight plans available offline
***

1. On the iPad mini, open up DroneDeploy.
    - The interface is the same as on the web browser.
2. While connected to the internet, navigate to your project.
    - The projects you created on the web browser should sync automatically.
3. Select the plan you want to make available offline.
4. Turn off Automatic Settings
5. Select the toggle for 'Make Available Offline'
6. Allow plan to fully sync before closing the app.
7. Before heading into the field, make sure that your plan is downloaded for offline use.
    - Turn on airplane mode
    - Close the app
    - Re-open the app and ensure its available and displaying properly.
    - You can also restart the iPad and repeat steps above.

## Uploading imagery to Box and DroneDeploy (Post-Flights)
***

[Video Tutorial](https://youtu.be/Dx-pgS56O6g)

1. Create a folder on Box to house all of your drone data.
  - This folder should be named after the month and year that the imagery was captured (i.e. June\_2023)
  - Within the 'Month\_Year' folder you should create separate folders for each flight that was captured in the field.
  - Within those folders you should create the following folders:
     - Elevation: _houses the elevation models from DroneDeploy_
     - Geomorphic\_Mapping: _houses the mapping that is done later on_
     - Obliques: _houses the oblique imagery that was captured in the field_
     - Orthoimagery: _houses the high-res orthoimage from DroneDeploy_
     - Raw: _houses the individual images from the field prior to mosaicking

2. Delete ground photos.
    - Prior to takeoff, the drone always takes a photo of the ground. Go through and delete these photos from the SD card.
3. For each flight, move the oblique photos from the SD into the relevant 'Oblique' folders.
4. For each flight, move the raw photos from the SD into the relevant 'Raw' folders.
5. In DroneDeploy, navigate to the relevant project and press the 'Upload' tab at the top of the screen.
6. Drag and drop your photos from the 'Raw' folder into the upload pane.
    - After the upload is complete, the images need to be processed by DroneDeploy before the products will be available for export. This can take a few hours.

## Exporting DroneDeploy products
***

1. Once the processing has been completed, you can access the available data by clicking the 'Explore' tab and navigating to the date that the images were collected.
2. From there, click the 'Export' icon at the bottom left of the screen
3. Select the product you want to export.
    - The two products we will almost always export are the GeoTIFF Mapp (which is the orthoimage) and the DTM.
4. Exporting the Orthoimagery.
    - Select the GeoTIFF option.
    - Change the email address from Wally's email to yours.
    - Make sure the file type is GeoTIFF.
    - Change the resolution to 2 in/px.
    - Click 'Export'.
5. Exporting the DTM
    - Select the DTM option
    - Change the email address to your email
    - **Make sure file type is** **Raw Elevation Values (DTM)**
    - Click 'Export'
6. Once you select 'Export' the products will begin processing. Once the processing is complete you will receive an email from drone deploy with a link to download the product. Save each product into their designated folders on Box
    - Orthoimage goes to the Orthoimagery folder
    - DTM goes to the Elevation folder

## Other Resources
***

DroneDeploys documentation on flight planning

[**https://help.dronedeploy.com/hc/en-us/articles/1500004964302-Mobile-App-Flight-Planning**](https://help.dronedeploy.com/hc/en-us/articles/1500004964302-Mobile-App-Flight-Planning)

DroneDeploys documentation on exporting data

[**https://help.dronedeploy.com/hc/en-us/articles/1500004964642-Exporting-Your-Data**](https://help.dronedeploy.com/hc/en-us/articles/1500004964642-Exporting-Your-Data)