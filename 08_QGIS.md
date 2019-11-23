### Chapter 8: QGIS

#### 8.1 Introduction to QGIS

QGIS as a light-weight, open source and free GIS software, is very popular for designers and developers. However, without data, it is no way to use it. This article will introduce you multiple tricks to get geological data. The version I use in this tutorial is QGIS 3.2.3-Bonn. New version integrated multiple plugins, which makes QGIS much convenient.

QGIS作为一款免费的轻量级的开源GIS软件深受设计者欢迎。巧妇难为无米之炊，没有数据，没有资源QGIS就没办法发挥其优势。如何获取地理数据资源的问题本文将重点介绍和讨论。本文用的QGIS版本为 3.2.3-Bonn, 新版本整合和多个插件，使得使用更加方便和人性化。

#### QGIS获取地理数据方法一：XYZ Tiles

在Browser里有各种获取网络数据的方式其中一栏为 XYZ Tiles. 其本身已经自带了OpenStreetMap, 可以直接拉到Layers或显示框里来显示OpenStreetMap。除了OpenStreetMap, XYZ Tiles 可以添加各种网络地图来使用，只要右键XYZ Tiles选择New Connection... 填写Name和URL即可。 所有可添加的URLs可以在这里查看到：

https://wiki.openstreetmap.org/wiki/Tile_servers

为了方便这里可以使用Python代码一键添加多个资源，代码由 Klas 提供：

[代码](https://raw.githubusercontent.com/klakar/QGIS_resources/master/collections/Geosupportsystem/python/qgis_basemaps.py)

拷贝此链接打开的代码，然后直接点击界面工具栏的 Python Console 图标，将代码粘贴到输入栏里按回车键就完成运行了！再次点开XYZ Tile 你会发现各种各样的地图资源，直接拉进图层或地图框里即可显示。此资源列表包含地形，卫星，海洋，云层，气温，黑暗风，水彩风等地图，可以自己探索一下。

#### QGIS获取地理数据方法二：ArcGisFeatureServer

ArcGisFeatureServer 是从 ArcGIS 的 REST API 来获取数据的工具。 美国有非常多的当地政府网站使用 REST API 来以动态网页地图的方式公开当地的地理信息，如建筑，街道，洪水，地形等。一般这种当地的信息是最新更新的，比较详细权威。 例如：

Jefferson Parish 区域地理信息http://geoportal.jeffparish.net/public

New Orleans 区域地理信息 http://property.nola.gov/

问题在于动态网页地图只显示图片结果，无法直接下载数据信息。如何爬取后台数据并导入QGIS，接下来将以一个网站为例一步一步讲解： 首先打开以上其中一个网页，可以看到地图显示，然后将浏览器打开开发者工具Developer Tools（Chrome 或者 Firefox 可以按快捷键 Ctrl/Command + Alt + i ），看到有一项目栏为 Network，点击后会有二级项目栏，从All 切换到 Img, 然后就会出现网页载入的地图图片链接，右击任意一个并复制其URL链接地址，复制出来的链接格式类似如下：

https://gis.nola.gov/arcgis/rest/services/Staging/Addresses/MapServer/export?dpi=...... ......

或者：

http://webmap.jeffparish.net/arcgis/rest/services/CODE/Code_Enforcement/MapServer/export?dpi=...... ......

我们只需要截取到export前面的链接就够了，例如：

https://gis.nola.gov/arcgis/rest/services/Staging/Addresses/MapServer/

或者：

http://webmap.jeffparish.net/arcgis/rest/services/CODE/Code_Enforcement/MapServer/

复制截取过的链接，打开QGIS，右击ArcGisFeatureServer，新建New Connection。在Name栏命名你的数据，URLs栏粘贴进我们截取好的链接，最后Add添加即可。添加完后就可以在ArcGisFeatureServer栏下找到刚添加的数据列表，展开后是各种数据图层，拉入你想要的图层即可。因为要临时从网络获取数据，大区域完全载入可能会比较慢。等图层完全载入完毕，我们就可以右击图层导出数据以备将来使用，导出有各种格式的数据包括dxf, shp, csv, json,kml 等等 导出后载入其他软件进一步处理，十分方便。

#### QGIS获取地理数据方法三：使用WMTS获取MapBox自定义风格地图

MapBox是一个可以为网站和应用自定义在线地图的公司。由于它的丰富度和自由度和艺术性相对于乏味的传统在线地图有巨大的优势，深受市场和使用者追捧。可惜MapBox对于导出高分辨率地图有一定限制，商业用户有50次机会，普通用户只有有5次机会。通过QGIS的WMTS功能可以加载MapBox的地图并绕过其限制。

操作过程如下：

由于WMTS只识别固定格式的链接，首先我们需要编辑出争取的链接，下面是链接的格式：

```
https://api.mapbox.com/styles/v1/YOUR_USERNAME/YOUR_STYLE_ID/wmts?access_token=<your access token here>
```

你需要做的就是将链接里的YOUR_USERNAME换成你MapBox账户的名字，YOUR_STYLE_ID换成你地图风格的ID号，将改为你的进入秘钥，这三个信息其实可以风格列表项目的 Share&Use 的链接里找到；或者在风格列表项目的 Menu -> Style URL找到USERNAME和STYLE_ID，在账户账户管理页找到你的秘钥。

链接编辑好后，打开QGIS，右击WMTS建立新连接，然后填写名称和我们准备好的链接添加即可。 添加好后就可以直接拖进地图或者图层进一步查看，编辑或者导出啦。

#### QGIS获取地理数据方法四：各大地理信息数据网站

这里主推一个网站：[Geospatial Data Gateway (GDG)](https://datagateway.nrcs.usda.gov/)

它包含了美国各州所有的地理信息数据，包括人口，降雨，气温，气候，用地，河流，农业，地形等等 数据十分全面和详细，尤其是地形的原始数据。选择数据下载时，选择的数据有时会过大，需要缩小所选区域再下载。

获取数据的步骤如下：打开[Geospatial Data Gateway (GDG)](https://datagateway.nrcs.usda.gov/)，点击绿色的按钮Get Data，进入选择你要获取数据的区域。有两种方法，一种是选择State再选County; 另一种点击链接Here直接在地图上框出你要的区域。推荐使用第二种，更将准确并节省资源。选好后会出现所选区域有哪些更够获取的数据，勾选你想要得数据，提交订单。过程中可能会需要你的邮箱及个人信息。提交完成会有订单号可以查询订单状态。等数据处理好后，系统会发邮件提醒你下载。一般会比较快几分钟到十几分钟，有事也会遇到一两个小时的情况。数据链接有效期为一星期，过期后需要重新选择数据提交订单。