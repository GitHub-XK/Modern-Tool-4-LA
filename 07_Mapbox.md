Chapter 7: Mapbox

If we say the OpenStreetMap is the Data Resource, the Mapbox is the beautification of the data, or application of the data. The map data in Mapbox is basically coming from the OpenStreetMap. Google map, OpenStreetMap, BingMap, Apple Map only have 2 or 3 different view themes, while Mapbox could have infinite styles of maps and various combination of data sets. 

7.1 Introduction to Mapbox

7.1.1 What is Mapbox?

Mapbox is the location data platform for mobile and web applications. They provide building blocks to add location features like maps, search, and navigation into any experience you create. (https://www.mapbox.com/about/)

In another word, Mapbox can help people customize their own map, and apply the map into website, smart phone application, games, augmented reality... 

Since it mainly aimed to technology or internet related companies, how could it used by landscape architects? While, you could think it as an GIS beautification tool, like an illustrator to visualize the data of OpenStreetMap. In landscape design, we could use it to build beautiful base map for project site analysis or master plan renderings. Comparing to traditional process (GIS -> CAD -> AI), using Mapbox simplifies the processes of finding , organizing, cleaning map data, and stylizing linework, polygon area and labels. Once familiar with the use of Mapbox, it could help you quickly produce the drawing.



7.1.2 Mapbox Studio - Styles, Tilesets, Datasets

(https://docs.mapbox.com/studio-manual/overview/) 

If you like to start your own map, Mapbox Studio is the tool you should definitely try. However, you need an account first before you could access anything. After login, Go to the page of [Mapbox Studio](https://studio.mapbox.com/). Here you can start your new style from multiple templates.  After building, your map will show on your styles list.

There are three main functions showing on the top tabs of the Mapbox Studio: Styles, Tilesets, and Datasets. Styles is what we would use most frequently, Tilesets and Datasets is designed for users who need to add customized data over the native datasets. 

In datasets, you could create new dataset by adding points, strings, polygons, images into the map. Dataset save your data abstractly. Tilesets is the tool that can convert the abstract data to graphics. Go to the page of Tilesets, create a new tileset by importing the previous dataset. In the tileset editor, you could visualize its looking at 22 preset zoom levels. 

Final step, switch to Styles tab, open the specific styles you created or the default templates, then add the customized tilesets into your map and adjust the looking.

The final step to import customized data into styled map is to add the tileset into the styles you created by styles editor. 

7.1.3 Examples of Mapbox Style

[Mapbox Gallery](https://docs.mapbox.com/studio-manual/examples/) provides many beautiful style examples, for instance the Decimal, Blueprint, Ice Cream and so on. Check your favorite style, and build your own map from it. 





7.2 Simple Guild to Mapbox (https://docs.mapbox.com/)

After brief introduction of Mapbox, a detailed tutorial will teach you how to build your own map step by step. 

7.2.1 Add Customized Data

For example, you would like to create a map showing all the locations of died tree of an area. You could add customized point data with its properties like name, condition, species, and notes, on the existing map through Datasets of Mapbox Studio. Starting with a new dataset in Mapbox Studio, 

7.2.2 Customized Map Style



7.2.3 Add 3D Building

7.2.4 Mapbox SDK in Unity



Frequently Asked Question (FAQ)

