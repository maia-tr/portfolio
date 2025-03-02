---
title: Land Surface Temperature in Szczecin, West Pomerania (Poland)
nav_order: 2
has_toc: false
---

## Land Surface Temperature in Szczecin, West Pomerania (Poland)

### Overview
Here I showcase effects of geospatial analysis dedicated to environmental and urban studies in Szczecin, Poland. This project is designed to practice geospatial data analysis skills and showcase data visualizations, focusing on themes related to urban climate, vegetation health, and land use and it aims to provide insights into environmental changes and urban dynamics.

### Objectives

This project serves as a space for practice of geospatial analysis and visualization, with a focus on the following objectives:
- developing spatial and non-spatial data analysis skills
- gaining experience with tools like QGIS, Google Earth Engine and Python libraries commonly used in geospatial science
- experimenting with data analysis and visualization tools
- providing visualizations and insights on topics significant to the health and state of the natural and urban environment

### Exploring Land Surface Temperature (LST) - description of a process


**Defining area of interest**

First I had to define Area of Interest, which was Szczecin's administrative boundary. It was obtained by using Overpass Turbo to query OpenStreetMap data. After downloading, these files were imported into QGIS for initial cleaning. This step included: Removing boundaries for a different, smaller town in Poland also named Szczecin and deleting unnecessary map layers, such as deanery boundaries, to focus solely on neighborhoods within Szczecin city.

**Data Acquisition**

Then the cleaned Szczecin boundary shapefile was uploaded to GEE. I retrieved Landsat imagery with Land Surface Temperature data via Google Earth Engine. I ended up having one thermal raster image from August 24, 2024. This date was selected as it falls in the summer, with clear skies over the city, providing an optimal LST measurement without interference from cloud cover out of the available images from the period of time 1.06.2024-31.08.2024.

Moreover, I added the population data, which I obtained from Szczecin's wikipedia page. I wanted to provide a little bit more information about population density in neighborhoods for more context. 

**Main outputs**

#### Mapping mean LST per neighborhood, with a tooltip showing basic zonal statistics with population density. To do so I perfomed following calculations:
	- descriptive statistics of LST (min, max, mean) per neighborhood
	- the area in square kilometers of each neighborhood and then population density per neighborhood
[see the map](https://maia-tr.github.io/portfolio/lst/zonal_stats_map.html)

#### Mapping LST values for each pixel while hovering over it I with the use of Bokeh Python library. It was needed to do following tasks to prepare the map:
	- first mapping LST values from a raster file onto polygons that represent individual pixels
	- calculating x and y coordinates from polygon geometry
[see the map](https://maia-tr.github.io/portfolio/lst/interactive_bokeh_plot.html)

**References**

- [Introduction to Remote Sensing of the Environment](https://github.com/geospatialeco/GEARS/blob/master/Intro_RS_Lab3.md)
- [Create and visualize Choropleth map with Folium](https://medium.com/analytics-vidhya/create-and-visualize-choropleth-map-with-folium-269d3fd12fa0)
- [Introduction to Python GIS](https://automating-gis-processes.github.io/CSC18/index.html)
- [Geopandas documentation](https://geopandas.org/en/stable/index.html)
- plenty of different youtube tutorials for GEE, no links sorry, but thanks to the people who shared them
