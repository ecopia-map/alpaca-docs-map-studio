**********************
Interface Walkthrough
**********************

Maps Tab
---------------

The Maps tab serves as the central administrative hub for creating and customizing 2D/3D maps, leveraging uploaded data and layering datasets to achieve the desired visualizations. This tab offers flexible publishing options tailored to user requirements, enabling optimal map delivery and presentation.

From the map page you can create, edit, and see information about any of your created and public ready maps with styles and find links for using your style template in web and mobile applications.

.. figure:: /images/map-studio/maps-tab.png
   :align: center
   :alt: Illustration of Maps Tab
   :width: 550


Create New Maps |newmapbutton|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you would like to build new maps, you can click on the :guilabel:`New Map` button locate on the right top of the Map List. You will be able to select from 2D or 3D maps.

* 2D map story will allow you to add 2d vector layer and 2d imagery tiles for your maps.
* 3D map scene will allow you to add a 3d vector layer and 3d imagery and 3d terrain to demo a 3d scene for your project.

to create a new map, simply select from 2D and 3D and select the templates from below and click on the :guilabel:`Create` button.

.. figure:: /images/map-studio/create_map.gif
   :align: center
   :alt: Example of usage purpose created for a content
   :width: 450


.. note::

	As of now, our system only provides a blank map as the default configuration option. In the near future, we intend to improve the user experience by offering a variety of built-in templates, allowing users to construct their maps with greater ease.

Map List
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /images/map-studio/Map-List-Item-Components.png
   :align: center
   :alt: Map List Item Illustration
   :width: 550

   *Map List Item Illustration*

Each listed map is composed of below components:

   #. :guilabel:`2D` / :guilabel:`3D` **Label**
   #. **Map Preview Thumbnail**: captured by :ref:`tools:Capture View Tool |Capture_preview_button|`
   #. **Map Title**
   #. **Relative time and action details**: This is a brief summary of the relative times of modification and publication for this map.
   #. **Preview Button** |preview_button|: Click on this button will open the Map Style Editor that allow you to modify the style of the map.
   #. **More Actions Button** |more_action_button|: Click on this button will allow you to do the below actions:

   * :guilabel:`Duplicate` Duplicate this map with same settings but unpublished.
   * :guilabel:`Publish` (Only displayed with published maps) Copy publishing information:

         * Shared users will be able to view the map with the link in the pop-up link by providing the access token. 

            .. figure:: /images/map-studio/publish_info.png
               :align: center
               :alt: Map List Item Illustration
               :width: 550

   * :guilabel:`Delete` : Delete this map permanently.

.. Note:: For more information about how to publish and generate a link to map demo, please refer to :ref:`howtos/CommonOperations:Generate Access Link to Demos`. 

Map Details Panel
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /images/map-studio/detail-panel.png
   :align: center
   :alt: Example of a Map Details Panel
   :width: 550

This panel will shows more details with a large thumbnail image of the highlighted map that you clicked on, below are the components of the Map Details Panel:

   * **Map Title**: This is the Map Title that can be set up in the Map Style Editor.
   * **Map ID**: This is the unique ID that can be used to identify this map.
   * **Map Preview Thumbnail**: This preview thumbnail can be captured using the Preview Capture tool in the Map Style Editor.
   * **Detail Settings**:

      * **Types of the map**: We have 2D Map Story and 3D Map Scene as the two default Map Type.
      * **Date Added**: The Date and timestamp of map was created and added to Map Studio.
      * **Date Updated**: The Date and timestamp of this map when it was last edited.
      * **Publish Status**: The Status of whether this map is published or not.
      * **Download link of demo HTML file**: The demo HTML file that can be used to visualize the stylized map in your local or your own host.

|

Map Style Editor
-----------------------

The Map Style Editor can be accessed through the Preview Button |preview_button| listed in the Map List of the :ref:`tools:Maps Tab`.

.. figure:: /images/map-studio/map_style_editor.png
   :align: center
   :alt: Example of Map Style Editor
   :width: 550

   *Layout Demo of a 2D Map in Map Style Editor*

General Tools in Map Style Editor:

  * :ref:`tools:Map Title Editing`
  * :ref:`tools:Tileset Panel |Tileset_button|`
  * :ref:`tools:Base-map Panel |Base_Map_button|`
  * :ref:`tools:Search Location Tool |Search_Location_button|`
  * :ref:`tools:Capture View Tool |Capture_preview_button|`
  * :ref:`tools:Publish Map Tool |Publish|`

.. figure:: /images/map-studio/3d_demo_map_style_editor.png
  :align: center
  :alt: Example of Map Style Editor
  :width: 550

  *Layout Demo of 3D Map Specific Tools in Map Style Editor*

3D Scene Map Specific Tools in Map Style Editor:

  * :ref:`tools:2D-3D Map Attachment Tool |link_button|`
  * :ref:`tools:Set Lighting Time Tool |Clock|`

Map Title Editing
~~~~~~~~~~~~~~~~~~~~~~~~~~

Map title can be edited by clicking on the edit button.

 .. figure:: /images/map-studio/name_map.gif
    :align: center
    :alt: Example of Map Style Editor
    :width: 350

    *Demo of how to change Map Title*

Tileset Panel |Tileset_button|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tilesets, on the other hand, provide a powerful data management solution that streamlines the import of data from local drives or S3 into the Map Studio Appilcation. This process is pivotal to the composition of maps within the Maps tab.


Tileset Panel is designed for add vector tiles into the map. Tileset Panel is composed of the below tools:

  * :ref:`tools:Add Vector Tileset Tool |Add_Tileset|`
  * :ref:`tools:Properties Tool  |propertiesbutton|`
  * :ref:`tools:Style Options Tool |stylebutton|`
  * :ref:`tools:Label Tool |labelbutton|`

Add Vector Tileset Tool |Add_Tileset|
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

New tilesets with type **2D Tiles** and **3D Tiles** can be added by clicking |Add_Tileset| button. In the new window, users can select the tilesets that are created by them or shared by other users.

 .. figure:: /images/map-studio/Add_Tileset_Vector.gif
    :align: center
    :alt: Add Tileset
    :height: 360


    *How to Add Tileset*

Properties Tool  |propertiesbutton|
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Property tools allow users to adjust following settings for layers in the map:

   1. **Transparency**: adjust the transparency of map layers

   2. **Visibility Range**: adjust the visibility on different zoom levels 

   3. **Attribute**: Edit layer style

.. figure:: /images/map-studio/properties_tool.png
   :align: center
   :alt: Example of properties tool
   :width: 360

   *Adjust Properties*

Style Options Tool |stylebutton|
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Ecopia’s Map Studio allows users to customize the display properties of geospatial layers. Users can change the colour, transparency, and border (if applicable) of layers by using the style option tool. With the Styles tab under Styles Options tool opened, users can modify the style of their layer as they see fit.

Layer features can be categorically styled based on a field in your data. Random colours will be assigned to features with different field values and features with the same field value can be styled together. 

Styles Available:

   1. **Categorized**: colours will be assigned to features with different field values and features with the same field value can be styled together. 

   2. **Single_Symbol**: one colour style that applies to all features in the map

.. figure:: /images/map-studio/style-editing.png
   :align: center
   :alt: Example of style option tool
   :width: 360

   *Style Editing*

Label Tool |labelbutton|
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Label tools allow users to display features' attributes value based on selected attribute. In addition to the options of turning on/off label and choosing attributes, users can also adjust colors, size, fonts, and style.

.. figure:: /images/map-studio/label_tool.png
   :align: center
   :alt: Example of label tool
   :width: 360

   *Label Editing*

Base-map Panel |Base_Map_button|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Users can add and manage raster layers (imagery or terrain model). Visibility of individual raster asset can also be switched on/off from here.

.. figure:: /images/map-studio/Base_map_panel.png
   :align: center
   :alt: Example of basemap panel
   :width: 550

   *Basemap Panel*

Add Basemap Tileset Tool |Add_Tileset|
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

This tool can be used to add tileset type with **Raster terrain** and **Raster Imagery**. Users can add raster tileset from the existing list or the ones that are shared by other members of the platform.

 .. figure:: /images/map-studio/Add_Tileset_Raster.gif
    :align: center
    :alt: Add Tileset
    :height: 360


    *How to Add Raster Tileset*

Search Location Tool |Search_Location_button|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This Search Location Tool is similar to the Search Location Tool in Map Browser, when you click on the icon, there will be a floating tool display on the right-corner of the Map Viewer.

when you entered a valid latitude and longitude pair into the Search Location Tool, the Map Viewer will pan to that coordinate.

.. figure:: /images/map-studio/search_location_tool.png
   :align: center
   :alt: The search location tool demo
   :width: 500

   *Lat/Long Input Box*


Set Lighting Time Tool |Clock|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /images/map-studio/Set_Lighting_Time_Tool.png
   :align: center
   :alt: The search location tool demo
   :width: 500

   *Set Lighting Time Tool*

Capture View Tool |Capture_preview_button|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

You can click on this tool when the Map Viewer is showing the desire thumbnail of the map. The preview of the captured view will updated in the Maps Tab regarding the map.

Captured view for preview / thumbnail is displayed in the detail information panel and the left side of the map list.

.. figure:: /images/map-studio/Demo_capture_view.png
   :align: center
   :alt: The search location tool demo
   :width: 500

   *Capturing View for Thumbnail*

2D-3D Map Attachment Tool |link_button|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

2D-3D Map Attachment Tool allows users to bind 3D map with 2D map, which provide users with the capability to switch between 2D and 3D for target area.

By clicking the link icon |link_button| on the top right corner of the page, a list of available tilesets for binding will be listed. By clicking on the link icon |link_button|, on the right of selected tilesets, the corresponding 2D layers will be bound with the 3D map.

.. figure:: /images/map-studio/Attach_3D_to_2D.png
   :align: center
   :alt: The Attachment of 3D scene to 2D story
   :height: 420

   *Link 2D-3D Map*

To unlink a 2D map from 3D map, click on |Cancel| button in the **Bind a 2D Map** window. The existing linked 2D map will be unbound.

Publish Map Tool |Publish|
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

By clicking on |Publish|, the current style settings will be applied to all hosting and published map that originated from the current map.

Settings:

   * **Default show map**: select the default map view, 2D or 3D;
   * **Show tileset layer panel**: switch to determine whether tileset layer panel will be displayed in the published map
   * **Show imagery layer panel**: switch to determine whether imagery layer panel will be displayed in the published map
   * **Show terrain layer**: switch to determine whether terrain layers will be displayed in the published map
   * **Hide imagery layer by default**: switch to determine whether the imagery layer will display by default in the demo
   * **Hide terrain layer by default**: switch to determine whether the terrain layer will display by default in the demo 
   * **Show vector layer panel**: switch to determine whether the vector layer panel will display by default in the demo
   * **Show raster layer panel**: switch to determine whether the raster layer panel will display by default in the demo 
   * **Support select feature**: switch to determine whether selecting feature is allowed in the demo
   * **Control vector layer opacity**: switch to determine whether the vector layer opacity can be adjusted in the demo
   * **Upload logo**: logo file that will be combined with the demo
   * **Company Name**: name of the Company

.. figure:: /images/map-studio/Publish_Map.png
   :align: center
   :alt: Publish map tool interface
   :width: 600

|

Tilesets Tab
---------------

.. figure:: /images/map-studio/tilesets_layout.png
   :align: center
   :alt: Sample Layout of Tilesets Tab

   *Layout of Tilesets Tab*


The Tileset Tab has the following components: 

  * :ref:`tools:Add New Tileset Tool`: Create new tileset and add to the existing tileset list
  * :ref:`tools:Tileset Table` : Table view of information of all available tilesets under this account
  * :ref:`tools:Tileset Detail Information Panel`: Detailed information display of a single tileset



Add New Tileset Tool
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The New Tileset can be upload and add to the Map Studio from the Ecopia Map Platform Drives or from the S3 of Amazon.

Below are the illustrations of both way of adding new tileset to the Map Studio.


Add New Tileset from My Drives
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. figure:: /images/map-studio/addnewtilesetfromdrive.png
   :align: center
   :alt: Sample Layout of Tilesets Tab
   :width: 500

   *Dialog of Add New Tileset from Drives*

The following fields need to be filled to create a new tileset from my drive:

   * **Asset Name**: provide tileset with desired name
   * **Description**: provide some description of the data that is being used to create this tileset
   * **Asset Type**: specify the type of data that is used for this tileset
   * **Asset Path**: provide path information for tileset from “My Drive” on the platform.

Add New Tileset from S3
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. figure:: /images/map-studio/addnewtilesetfroms3.png
   :align: center
   :alt: Sample Layout of Tilesets Tab
   :width: 500

   *Dialog of Add New Tileset from S3*

If users choose to create new tileset from S3, the following addtional information is required:

   * Asset Type
   * Access Key ID
   * Secret Access Key
   * Bucket
   * Prefix 

Tileset Table
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The uploaded tilesets will be presented in a tabular format, including fundamental details about each one. To access further information about a specific tileset, simply click on it, the selected tileset will highlighted in light-blue and a detailed information panel will appear on the right-hand side of the window.

Tileset Type
^^^^^^^^^^^^^^^^^^^^

There are four types of tileset (Asset) are supported in our platform:

* **2D Tiles (mvt)** - 2D vectors in shapefile format (zip)
* **3D TIles (tileset)** - 3D vectors in shapefile format (zip) with height attributes. Two of the following three values need to be spcified in the shapefile attributes to create the tileset: 
   
   * **Abs Height** - height of the building roof above sea level
   * **Rel Height** - height of the building itself
   * **Dtm Height** - height of the button of the building above sea level
   
* **Raster Terrain** (terrain_provider) : This is a Base Map Type that shows the terrain shape of the map area
* **Raster Imagery** (imagery_layer) : A type of base map that shows the satellite imagery of the map area


Tilesets Actions
^^^^^^^^^^^^^^^^^^^^^

  * :guilabel:`Delete` : Delete this tileset permanently.

  * :guilabel:`Rename` Rename the tileset.
  * :guilabel:`Share` Share this tileset with other accounts
  * :guilabel:`Make it Public` Change the Accessibility level to other users.

Tileset Detail Information Panel
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /images/map-studio/Tileset_detail_panel_layout.png
   :align: center
   :alt: Layout of Tileset Detail Panel
   :width: 500

   *Layout of Tileset Detail Panel*

This panel is silimar to the map detail panel, it will shows more details with an interactive preview of the highlighted tileset that you selected, below are the components of the Map Details Panel:

   * **Tileset Title** This is the Map Title that can be set up in the Map Style Editor.
   * **Tileset ID**: This is the unique ID that can be used to identify this map.
   * **Interactive Tileset Preview**: This is an interactive preview box to help you browse the converted tileset in a quick and simple way.
   * **Detail Settings**:

      * **Types of the tileset**: We have 2D Map Story and 3D Map Scene as the two default Map Type.
      * **Date Added**: The Date and timestamp of this tileset was created and added to Map Studio.
      * **Date Updated**: The Date and timestamp of this tileset when it was last edited.
      * **Publish Status**: The Status of whether this tileset is published or not.
      * **Download link of demo HTML file**: The demo HTML file that can be used to visualize the tileset in your local or your own host.

Asynchronous Job Window
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
The Asynchronous Job Window is located in the lower right corner of the window, it shows the progress of each upload task (tilesets), and you can track the progress.
You can also see this async job in the upper right corner of the Ecopia map platform to keep track of your queued async jobs.

|

Tokens Tab
-----------------------

The Tokens tab provides comprehensive control over map accessibility, serving as the primary command center for managing all published maps. Through this tab, users can fine-tune their map offerings, ensuring that the appropriate audiences have access to the right maps at the right time.

An access token provides access to Map Studio resources on behalf of a user. All user accounts have a default public token named default_token. Additional tokens can be created to grant additional, or more limited, privileges.

Create New Tokens
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To create the authorization token, click on :guilabel:`New Token` button.

.. figure:: /images/map-studio/create_token.png
   :align: center
   :alt: Example of usage purpose created for a content
   :width: 500

   *Create New Token*

The following settings are available for users to customize the new token:

   * **Name**: name for the token
   * **Description**: short description for the token
   * **Token Scope**: access control to available map stories/demos. Select stories/demo from the list of which can be accessed via this token.

Access Token Table
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: /images/map-studio/access_tokens.png
   :align: center
   :alt: Example of usage purpose created for a content

   *Access Token Table*

The Access Token Table is listing all the tokens have been created by the user. Users can view all information of all tokens in use.

Token scope
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Token’s accessibility to map contents are based on Token Scopes. Users either determine the token scopes by selecting the content that is available under this account during the token creation process or update token scopes later on.

Users can access and manage the token scope by clicking :guilabel:`Edit` in the access token table. In the token scope section, select maps that should be accessible via this token.

.. figure:: /images/map-studio/TokenScope.png
   :align: center
   :alt: Edit Token Scope
   :height: 420

   *Edit Token Scope*

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

.. |Cancel| image:: /images/map-studio/Cancel.png
    :height: 25