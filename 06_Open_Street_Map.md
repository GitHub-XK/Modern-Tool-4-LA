Part 3: Internet & Data

Introduction: Landscape architecture design can not build without accurate information. It is extremely important to access rich data set and analyze them before designing or implementing design solutions. In the past all the important information are stored at national agencies, like libraries, governments, geological department, and universities. Designers or publics often hardly could obtain these information. With growing of internet, and boosting of data and information, designers could easily access large amount of data without too much effort. However, because of the technology barrier, sometimes we don't know where and how to get them and convert to useful data that designer could use. For landscape architecture, geological data is extremely valuable and important. There are many sources and tools most of the landscape architects barely know where or how to use. This chapter will introduce several resources and tools that would essentially help designer to access useful data set.

Chapter 6: Open Street Map

6.1 Introduction to Open Street Map

6.1.1 What is Open Street Map(OSM)?

Ten years ago, paper map still was the major resource that provides accurate geographic and traffic information. Wherever you go, wherever you drive, a paper map is necessary for guiding the trip. The information from the internet was still very limited. Landscape architecture was getting the site information from the government, library, and related agency? As a generation of internet, I started my landscape career with rich public resource on the internet, especially by using google earth, online university library and some government website. However, sometimes, we still could not find information we need online, and had to find them on books and maps. Since the heat of big data and information boost on the internet in past five years. The most update, most accurate geographic information, all could be found on the internet with some efforts to dig it out. Beside google earth, there are way many new ways to get various data you want. And these new methods are seldom known by landscape architects. 

OpenStreetMap (OSM) is a collaborative project to create a free editable map of the world. The geodata underlying the map is considered the primary output of the project. The creation and growth of OSM has been motivated by restrictions on use or availability of map data across much of the world, and the advent of inexpensive portable satellite navigation devices. OSM is considered a prominent example of volunteered geographic information. (https://en.wikipedia.org/wiki/OpenStreetMap)(https://wiki.openstreetmap.org/wiki/About_OpenStreetMap)

6.1.2 Open Street Map vs. Google Map

(https://www.openstreetmap.org/user/jbelien/diary/44356)

(https://geoawesomeness.com/why-would-you-use-openstreetmap-if-there-is-google-maps/)



6.2 Usage of Open Street Map

6.2.1 Export Data & Analysis Data Format

First step is to get the Open Street Map Data directly from the website: [https://www.openstreetmap.org/](https://www.openstreetmap.org/). Search or zoom in the area you want to get data from, then click "Export" on the top left corner. The left page will show the range you select. Adjust the area, then click the blue "Export" button to download. If the blue "Export" button is not showing, it maybe meaning that the area you selecting is too big that exceed the export limit. You could either select a smaller area or download through "Overpass API". The expected format of the data file that you will download is ".osm". Once downloaded the osm file, it could be imported into different drafting or modeling software.

6.2.2 OSM to AutoCAD

AutoCAD is the most popular design drafting tool in the industry. However, there is no direct way to import .osm file to AutoCAD. The easiest way I found is to convert the .osm file to .dwg through some website like:

[https://mygeodata.cloud/converter/osm-to-autocad](https://mygeodata.cloud/converter/osm-to-autocad)

You could also directly extract, convert and download data in dwg format through this website instead of the openstreetmap website:

https://mygeodata.cloud/osm/data/download/

There is another convenient tool built based on open street map, CADMapper. You can directly download the site data in .dfx format through CADMapper. However, it is not free when your selected area is larger than 1 km2. 

https://cadmapper.com/



6.2.3 OSM to Rhino Grasshopper Elk

OSM also could be used as a base in 3d modeling software such as Rhino and Revit. In Rhino, there is a specific plugin, named Elk, to import and extract data from the .osm file through Grasshopper.

Rhino6 has native Grasshopper integrated, however rhino5 does not. Make sure the grasshopper is correctly installed for your Rhino. Then download and install the plugin "Elk" in [https://www.food4rhino.com/app/elk](https://www.food4rhino.com/app/elk). 

Open the Rhino, then open the Grasshopper. Find out where is the Elk menu located (It is usually located under "Extra" tab). Double click the blank working area, search and add "File Path" component. Right click "File Path" component to "Set One File Path", choose the .osm file we just downloaded. Then, add the components of "Location" and "OSMData" under the Elk menu. Connect the "File Path" to "Location", and connect the "Location" to "OSMData". ...PENDING

6.2.4 OSM to Revit Dynamo

Similar to Rhino, Revit needs Dynamo and Dynamo's Plugins to import OSM. The workable Dynamo's Plugins include: [[Elk for Dynamo / OSM to Mass]](https://dynamonodes.com/2016/04/26/workflow-building-masses-from-osm-files/#more-2229), [[DynaMap]](https://dynamobim.org/dynamaps/). 

6.2.5 OSM to QGIS

QGIS can directly import OSM as vector data, and categorize the data according to types like points, lines, and polylines.

6.2.6 OSM to SketchUp

There are multiple plugins could help SketchUp to import OSM data:

[[Sketchup-OSM-Importer]](https://github.com/m93a/Sketchup-OSM-Importer)

[[skp2osm]](https://wiki.openstreetmap.org/wiki/Skp2osm)

[[Three Ways To Import OpenStreetMap Data In SketchUp]](https://www.youtube.com/watch?v=KKUGAZXU4dY)



