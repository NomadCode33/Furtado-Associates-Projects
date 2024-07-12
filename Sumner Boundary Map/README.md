# Sumner Boundary & Raster Maps
Write a short sentence or two about this project and what it does. Be sure to include a link and a screenshot (we're front end devs so we can actually see our work!).

**Disclaimer:** Furtado & Associates maintains a policy of not allowing company property for personal use, so I don't have any documents or pictures of my project. However, I can describe the work I did and the process we followed.

## How It's Made:

**Tech used:** ArcGIS Pro, ArcGIS Online, Autodesk Civil 3D, Microsoft Excel, Office Database

### Sumner Boundary Map: A Journey Through Data Mapping

Creating the Sumner Boundary Map was one of my proudest achievements, a project I tackled independently without any outside assistance. The process began with opening ArcGIS Pro and understanding the project scope, which in this case, centered around the area of Sumner.

To ensure accuracy, I adjusted the coordinate system to align with Furtado’s specialized system, known for its precision. This meticulous approach is why many companies, including Sound Transit, prefer working with Furtado. They rely on our accurate and timely project completions.

I started by establishing the project boundary. Using ArcGIS’s polygon tool, I defined the boundary area and employed the Feature Class to Feature Class tool to incorporate and cleanse the data. This step is akin to inheriting older data and making it our own by refining and optimizing it for quicker loading and rendering, especially important for larger datasets. After adding the boundary to the database, I changed its color to red in the Symbology pane for clear visualization.

With the boundary set, the next step was gathering datasets. I scoured open sources like the county GIS portal and ArcGIS Online, searching for various data types, including GPS data, water systems, wastewater, storm drains, and other utilities. Verifying metadata was crucial, ensuring all data was accurate and relevant.

Using the ETL (Extract, Transform, Load) process, I cleaned and organized the data. The Feature Class to Feature Class tool helped transfer new data into my database for easy access. Checking the attribute table and metadata allowed me to filter data using the Select By Location and Selection By Attributes for Boundaries tools, ensuring only the relevant information was highlighted.

For example, to filter out culverts, I used the attribute table to select specific columns and create new layers from the selections. Each dataset had multiple types, necessitating further splitting for project clarity. Geographic coordinates were added when missing, using the Calculate Geometry Attributes tool to ensure accuracy.

The next phase involved integrating data from ArcGIS into Autodesk Civil 3D for better management and visualization. This integration allowed for precise area specifications and comprehensive project scopes. I used the Feature Class to Shapefile tool to export GIS data into Autodesk CAD software, organizing the data into specific folders for sanitary sewers, stormwater, and water, and further subdividing into points or line data.

In Autodesk Civil 3D, I imported shapefiles, starting with the map boundary, followed by other data types. Line values required plotting on the map, setting spatial filters, and assigning colors through the layer properties. Point values needed block standards assignment, ensuring each point type (e.g., hydrants, water valves) was correctly labeled and scaled for visibility.

Creating labels and pipes involved returning to ArcGIS Pro. I added new fields in the attribute table, calculated geometry attributes, and generated points along lines. These points were then exported to Excel for further processing. In Excel, new columns were added, merging data for easier label generation when transferred back to ArcGIS.

After refining the data, I imported it back into ArcGIS and matched everything to the original layers for label visibility in Autodesk Civil 3D. This meticulous process ensured each label was correctly placed and formatted. In Civil 3D, I finalized the labels, adjusting their properties, colors, and scales to match the utility classification layers.

### Creating the Raster Map

Next, I embarked on creating a raster map, which represented Sumner’s features and characteristics as a grid of pixels. I started by setting the map’s coordinate system in ArcGIS to Furtado’s custom system. Adding aerial data for Sumner and defining the project boundary with a bright red dashed line made it stand out.

For larger project scopes, subdividing boundaries was necessary to manage data efficiently. I added a new field in the attribute table, subdivided the polygon, and measured distances to create equal parts. These subdivisions were essential for converting the map into manageable raster tiles, ensuring faster rendering times.

With the boundary set, I prepared to create raster map files. Turning off unnecessary layers, I focused on the Sumner Aerial data, zooming to the desired tile. Exporting the layout as a GeoTIFF, I opted for a high resolution of 1000 DPI with a 32-bit color depth and a transparent background. This high-quality output was saved to my office database’s raster folder, ensuring detailed and accurate visual representation of the area.

Through this intricate process, the Sumner Boundary Map came to life, a testament to meticulous planning, precise data handling, and seamless integration across multiple platforms. Each step was a blend of technical skill and creative problem-solving, ensuring the final product was not only accurate but also visually engaging and easy to interpret.

## Optimizations

fdfdfdfd

## Lessons Learned:

No matter what your experience level, being an engineer means continuously learning. Every time you build something you always have those *whoa this is awesome* or *wow I actually did it!* moments. This is where you should share those moments! Recruiters and interviewers love to see that you're self-aware and passionate about growing.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Palettable:** https://github.com/alecortega/palettable

**Twitter Battle:** https://github.com/alecortega/twitter-battle

**Patch Panel:** https://github.com/alecortega/patch-panel
