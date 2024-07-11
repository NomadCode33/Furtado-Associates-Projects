# Sumner Boundary & Raster Maps
Write a short sentence or two about this project and what it does. Be sure to include a link and a screenshot (we're front end devs so we can actually see our work!).

**Disclaimer:** Furtado & Associates maintains a policy of not allowing company property for personal use, so I don't have any documents or pictures of my project. However, I can describe the work I did and the process we followed.

## How It's Made:

**Tech used:** ArcGIS Pro, ArcGIS Online, Autodesk Civil 3D, Microsoft Excel, Office Database

The Sumner Boundary Map was one of many boundary maps I have created, this however was one of two boundary maps that I did without receiving help. The process starts with opening up ArcGIS Pro and finding out the project scope specifications of where I've working in, in this case, Sumner. Next, I change the coordinate system to refer to the datum based off the scope of work so it can be accurate. Furtado uses their own specialized coordinate system which makes their work really accurate. It's due to this that a lot of companies like Sound Transit prefer working with them the most and how timely they are with their projects. I then create a project boundary which outlines the project scope I'm working in. I use a polygon tool with ArcGIS to set it over the boundary I'm working on. From there I use the Feature Class to Feature Class tool to take the newly added data and take ownership of said data from the original source, kind of like a hand me down from older siblings. It then takes the data and scrubs it to take whatever I want, it's like taking off the data of another person and inputting my own data. This also very handy since it causes the data to be easily used and that it doesn't take a long time to load and render, which is necessary for bigger datasets I find. This is one of the tools that will be used for cleaning the datasets that are added to the map view. I used the Feature Class to Feature Class tool to add the boundary I made into the database which I also changed the color to be red in the Symbology pane. If the boundary has a big area for a scope of work, then i would have to subdivide the boundary. However that step isn't used yet here so it will be talked about later.

Next I start looking for datasets, I looked from open datasets such as the county GIS portal to find data and also ArcGIS Online, I also look for data using the metadata as well. The types of data I found can range from GPS data, water, waterwaste, storm drains, culverts, etc. and I then use GIS database elements within ArcGIS to make it more usable. Either during or after data collection I then verfiy the metadata by accessing the Properties of said data and go to source tab which takes me to the link where the metadata is available. After the process is done, I start cleaning the data using ETL process (extracting, transforming, and loading). I use the Feature Class to Feature Class tool to have the new data on my database for 

Developed precise topographic maps in ArcGIS Pro using GPS data, aerial photography, and GIS database elements, similar to a utility network. Performed ETL processes to migrate water and wastewater data across systems and integrated it with Autodesk Civil 3D for efficient management and visualization. This enabled accurate area specifications, supporting comprehensive project scopes.

## Optimizations

fdfdfdfd

## Lessons Learned:

No matter what your experience level, being an engineer means continuously learning. Every time you build something you always have those *whoa this is awesome* or *wow I actually did it!* moments. This is where you should share those moments! Recruiters and interviewers love to see that you're self-aware and passionate about growing.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Palettable:** https://github.com/alecortega/palettable

**Twitter Battle:** https://github.com/alecortega/twitter-battle

**Patch Panel:** https://github.com/alecortega/patch-panel
