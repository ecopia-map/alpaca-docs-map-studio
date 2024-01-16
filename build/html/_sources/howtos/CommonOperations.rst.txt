**********************
Common Operations
**********************
This section covers some common operations within Map Studio.

Create Demo with Data on the Platform
######################################

Create New Tileset
======================================

Create New Map and Add Tilesets
======================================

Link 2D/3D Maps
======================================




Generate Access Link to Demos
######################################

**Step 1**: Under **Maps** tab, locate the map that is going to be used as demo, and click |more_action_button|

**Step 2**: Select **Publish** from the options

**Step 3**: In the pop-up window, copy the link under **preview only**, and paste it in Notepad

**Step 4**: Close **Publish** window, and navigate to **Tokens** tab

**Step 5**: Under **Tokens** tab, copy the corresponding token. 

**Step 6**: Go to Notepad, replace **{your-access-token}** string with the token that just copied in the map link

**Step 7**: Copy and paste the entire edited link to browser and hit enter. Notice that the demo is now showing in the browser


.. figure:: /images/map-studio/GenerateDemoLink.gif
   :align: center
   :alt: QGIS Add WMTS


   *Generate a Demo Link*



Create WMS/WMTS Tile Services for Imagery
##########################################

THis function allows users to quickly distribute the capability to view imagery data that is used to create the vector product. This function avoids the need to download the data as the WMS/WMTS can be easily access by common geospatial tools on the market.

**Step 1**: Go to the **Tileset** tab

**Step 2**: In the list below, locate the target imagery tileset. (To accelerate this process, users can filter based on **Type: Imagery**)

**Step 3**: Click on |more_action_button| button and select **Export to WMTS**

**Step 4**: In the pop-up window, click on :guilabel:`Create` to create a new tile service for this tileset

**Step 5**: In the next window, specify the value for **Valid day**, **Min zoom level** and **Max zoom level**. Then click :guilabel:`Commit`

**Step 6**: The window will return to **Export tile service list**, copy the WMTS link and load it to third party softwares

.. figure:: /images/map-studio/CreateWMTS.gif
   :align: center
   :alt: Create WMTS


   *Create WMTS Link in Map Studio*


The generated WMTS link should be compatible with most of the common geospatial analysis tools that are available on the market. The following section provides a step-by-step guide of loading WMTS via QGIS.

**Step 1**: Open QGIS and create a new project

**Step 2**: Go to the menu bar on the top of the window and navigate to **Layer** -> **Add Layer** -> **Add WMS/WMTS Layer..**

**Step 3**: In the prompt window, under **Layer** tab, click :guilabel:`New`

**Step 4**: In the prompt **Create a New WMS/WMTS Connection** window, specify the name of the connection and paste URL into corresponding field. Click :guilabel:`OK` to finish.

**Step 5**: From the dropdown, select the newly added WMTS and click :guilabel:`Connect`

**Step 6**: The window will switch to **Tileset** tab automatically, click on the imagery layer from the list to select. Click on :guilabel:`Add` to add the imagery tileset to the project

.. figure:: /images/map-studio/QGISAddWMTS.gif
   :align: center
   :alt: QGIS Add WMTS


   *Using QGIS to Add WMTS*



.. |propertiesbutton| image:: /images/map-studio/properties-icon.png
   :width: 28

.. |stylebutton| image:: /images/map-studio/style-icon.png
   :width: 22

.. |labelbutton| image:: /images/map-studio/label-icon.png
   :width: 24

.. |mapstudio| image:: /images/map-studio/map-studio-icon.png
    :width: 26

.. |newmapbutton| image:: /images/map-studio/newmap_button.png
    :width: 68

.. |more_action_button| image:: /images/map-studio/more_action_button.png
    :width: 22

.. |preview_button| image:: /images/map-studio/preview_button.png
    :width: 22

.. |Search_Location_button| image:: /images/map-studio/Search_Location_button.png
    :width: 22

.. |Tileset_button| image:: /images/map-studio/Tileset_button.png
    :width: 22

.. |Capture_preview_button| image:: /images/map-studio/Capture_preview_button.png
    :width: 22

.. |Base_Map_button| image:: /images/map-studio/Base_Map_button.png
    :width: 22
    
.. |link_button| image:: /images/map-studio/link_button.png
    :width: 26

.. |Add_Tileset| image:: /images/map-studio/AddTileset.png
    :height: 24

.. |Clock| image:: /images/map-studio/Clock.png
    :height: 24

.. |Publish| image:: /images/map-studio/Publish.png
    :height: 25