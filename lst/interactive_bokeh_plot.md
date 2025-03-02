---
title: "Interactive plot with Bokeh"
parent: Land Surface Temperature in Szczecin, West Pomerania (Poland)
nav_order: 1
---


#### **Interactive map of Land Surface Temperature in Szczecin** 
This is a very detailed map presenting LST data for each pixel in Szczecin area. While hovering over, one can see the LST value and the neighborhood name.
The map was done by mapping LST data from a raster file onto polygons representing individual pixels. 

<iframe src="{{ '/assets/lst_raster_to_polygons.html' | relative_url }}" width="100%" height="820"></iframe>

Python libraries used: Pandas, Geopandas, Rasterio, Bokeh