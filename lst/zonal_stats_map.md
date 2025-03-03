---
title: "Interactive choropleth map with zonal statistics"
parent: Land Surface Temperature in Szczecin, West Pomerania (Poland)
nav_order: 2
---

#### **Interactive choropleth map of LST mean values in each neighborhood** 
The map shows the mean LST for each neighborhood. Hovering reveals basic zonal statistics (mean, min, max temperature), as well as population density.

<iframe src="{{ '/assets/lst_zonal_stats.html' | relative_url }}" width="100%" height="580"></iframe>

Python libraries used: Pandas, Geopandas, Folium, Branca