# Sumner Boundary & Raster Maps
Write a short sentence or two about this project and what it does. Be sure to include a link and a screenshot (we're front end devs so we can actually see our work!).

**Disclaimer:** Furtado & Associates maintains a policy of not allowing company property for personal use, so I don't have any documents or pictures of my project. However, I can describe the work I did and the process we followed.

## How It's Made:

**Tech used:** ArcGIS Pro, ArcGIS Online, Autodesk Civil 3D, Microsoft Excel, Office Database

The Sumner Boundary Map was one of many boundary maps I have created, this however was one of two boundary maps that I did without receiving help. The process starts with opening up ArcGIS Pro and finding out the project scope specifications of where I've working in, in this case, Sumner. Next, I change the coordinate system to refer to the datum based off the scope of work so it can be accurate. Furtado uses their own specialized coordinate system which makes their work really accurate. It's due to this that a lot of companies like Sound Transit prefer working with them the most and how timely they are with their projects. I then create a project boundary which outlines the project scope I'm working in. I use a polygon tool with ArcGIS to set it over the boundary I'm working on. From there I use the Feature Class to Feature Class tool to take the newly added data and take ownership of said data from the original source, kind of like a hand me down from older siblings. It then takes the data and scrubs it to take whatever I want, it's like taking off the data of another person and inputting my own data. This also very handy since it causes the data to be easily used and that it doesn't take a long time to load and render, which is necessary for bigger datasets I find. This is one of the tools that will be used for cleaning the datasets that are added to the map view. I used the Feature Class to Feature Class tool to add the boundary I made into the database which I also changed the color to be red in the Symbology pane. If the boundary has a big area for a scope of work, then i would have to subdivide the boundary. However that step isn't used yet here so it will be talked about later.

Next I start looking for datasets, I looked from open datasets such as the county GIS portal to find data and also ArcGIS Online, I also look for data using the metadata as well. The types of data I found can range from GPS data, water, waterwaste, storm drains, culverts, and other types of utilities and I then use GIS database elements within ArcGIS to make it more usable. Either during or after data collection I then verfiy the metadata by accessing the Properties of said data and go to source tab which takes me to the link where the metadata is available. After the process is done, I start cleaning the data using ETL process (extracting, transforming, and loading). I use the Feature Class to Feature Class tool to have the new data on my database for easy access. I then check the attirbute table and metadata to see which variables are important for me to glean the information off of for analysis and for the things I'm gonna do. I then filter the data by using the Select By Location and Selection By Attirbutes for Boundaries tools. Select By Location tool tells ArcGIS Pro to select the data in said location and fit the data within it, in this case the data is fitted within the boundary that I made earlier. I right-click the layers that were selected and hovered over Selection then Create new layer from selected features. For the Selection By Attributes for Boundaries I select a specific area to fit to the scope of the work boundary, while being on the same layer that I selected, I attract specific types of the data within the layer using math terminology to find said types. For example, if I'm looking for culverts I select the featype_desc (or whatever column has this on different datasets on the attirbute table) is equal to culverts. It then filters out the culverts and I can create a new layer from the selection. Each datasets has multiple types so it's important to split them up for project purposes. I then feature the class to geodatabase to input the new trimmed layers that I made into the database for easy access. After sending it to the database, I filter it again if need be. If there is no location for the easting and northing or longitude and latitude, I add a field in the attribute table, put double for the data types, numeric for the number format, and I dothe same steps addinglayers for the other directions. I then match the northing or easting directions or even longitude and latitude as x or y coordinates depending on the native directions and ran it on the Calculate Geometry Attirbutes tool. Lastly, i change the symbology on the points to make sure that they are at the correct settings. 

Next up is integrating the data from ArcGIS into Autodesk Civil 3D for efficient management and visualization. Doing this enabled accurate area spedification, supporting comprehensive project scopes. I then used the Feature Class to Shapefile to export the GIS data into the Autodesk CAD software. I export the files into the office database of teh company and I sort my exported data into separate folder types. It goes from Sanitary Swers, Stormwater, and Water. In those three folders I then separate even further to points or line data. It will make it easier for the work I will do on Autodesk.



## Optimizations

fdfdfdfd

## Lessons Learned:

No matter what your experience level, being an engineer means continuously learning. Every time you build something you always have those *whoa this is awesome* or *wow I actually did it!* moments. This is where you should share those moments! Recruiters and interviewers love to see that you're self-aware and passionate about growing.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Palettable:** https://github.com/alecortega/palettable

**Twitter Battle:** https://github.com/alecortega/twitter-battle

**Patch Panel:** https://github.com/alecortega/patch-panel
