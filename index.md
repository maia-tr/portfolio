## Visuals for regional supply of senior clubs in Poland
Python libraries used: Folium, Pandas, GeoPandas, and Branca

#### **Interactive choropleth map** 
The map showcases number of places in senior clubs per 1,000 inhabitants for each commune.

<iframe src="{{ '/assets/interactive_map.html' | relative_url }}" width="100%" height="450"></iframe>

#### **Heatmap**
The heatmap presents the intesity of senior clubs across regions and hightlights high and low concentrations of places in senior clubs.

<iframe src="{{ '/assets/heatmap.html' | relative_url }}" width="100%" height="450"></iframe>


## Visuals for land surface temperature (LST) in Szczecin on 24th Aug 2024
Tools used: GEE, Python (i.a. Folium, Geopandas, Rasterio, Bokeh)

#### **Interactive map of LST** 
The plot was done by mapping LST data from a raster file onto polygons representing individual pixels. 

<div class="chart-container">
	<iframe src="{{ '/assets/lst_raster_to_polygons.html' | relative_url }}" width="100%" height="810"></iframe>
</div>

#### **Interactive map of mean land surface temperature in each neighborhood** 
The map shows the mean LST for each neighborhood. Hovering reveals basic zonal statistics (mean, min, max temperature).

<iframe src="{{ '/assets/lst_zonal_stats.html' | relative_url }}" width="100%" height="550"></iframe>