# Public / Open Source Tooling for Geographic Information Science/Analytics/Visualizations

This documentation lists useful tools for manipulating, analyzing and visualizing geographic information. By no means is this list exhausted, rather it's a list of all the tools I have used and I think would be useful for others who want to start leveraging geographic information. Sometimes a paid or enterprise solution (e.g., ArcEnterprise, Tableau) makes sense if your use case is visualizing geographic information, such as for reporting to policy-makers; but if conducting data collection or analytics, then an open source work flow would make more sense for transparency and reproducibility (e.g., R, Python). Throughout this document I specify what tools are more useful depending on your goal and data.

*For public servants: for those creating and working with geographic information, it is important to recognize that [TBS](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=16553) has set geographic data standards, hence there are metadata standards. These standards align with the [Open Geospatial Consortium (OGC)](https://www.opengeospatial.org/), an international is an international consortium which aims to make geogaphic information and services "FAIR - Findable, Accessible, Interoperable, and Reusable."*

Before jumping into geographic data visualization, I highly recommend reading the following blog posts on each of these foundational concepts in GIS:

TO DO: ADD LINKS

- Vector vs. Raster data models in GIS
- Projections
- Cartographic design

## Terminology

You'll hear Geographic Information Systems, Geographic Information Science, spatial analysis and spatial statistics.

In general, Geographic Information Systems (GIS) leverages geospatial data, statistical/analytical methods and technologies to interpret the “real world”. These technologies (e.g., paid or open source software or programming libraries) are used to store, retrieve, manipulate and display geographic data, but can also support analysis and statistics (further explained below).

Geographic Information Science (GIScience), on the other hand, studies data models and computational methods to collect, manipulate, process, analyze and visualize geospatial data. For example, studying methods for the following:
- Validating mining/crowdsourcing geospatial data
- Assessing the spatial distribution of spatially referenced social media posts
- Synthesizing big heterogeneous geospatial data (e.g., street level images + social media posts + infrastructure datasets) to assess accessibility

Spatial analysis and statistics, describes analytics and statistical concepts and methods that are conducted by Geographers (e.g. modifiable areal unit problem, spatial autocorrelation), which depends on a GIS. Spatial analysts, statisticians and scientists depends on a technical architecture to collect, store, manage, manipulate, run models, and visualize results.

## GIS Technical Architecture

The following is an example of a GIS. Esri's software offers an entire GIS, but with open source you can also build your own, and it's fairly easy now with a large international open source community developing the software and documenting its usage.

![GIS](./arc.png)



## Geographic Vector Data Structures

TO DO: ADD R PPPP SLIDES

## Geographic Open Data Sources
- [OpenStreetMap (OSM)](https://www.openstreetmap.org/), an international crowdsourcing project aimed at collecting an open source dataset of geographic information. Within Canada, there has been academic research to assess the quality of OSM data (Jacobs 2017; Zhang 2018)
  - Download OSM data from [Geofabrik](https://www.geofabrik.de/data/download.html), a web site that allows you to download the data in different formats and at different geographic scales (e.g., Canada, provincial, territorial, cities)
  - Contribute and download OSM data from [Java OSM (JOSM)](https://josm.openstreetmap.de/). JOSM is an open-source graphic interface to contribute, edit, validate OSM data, but can also be used to extract and visualize geospatial data as well
- Provincial and municipal open data portals
- [Statistics Canada boundary files](https://www12.statcan.gc.ca/census-recensement/2011/geo/bound-limit/bound-limit-eng.cfm) (e.g., Provinces/Territories, Economic Regions, Census Subdivision, Dissemination Areas)
- [Federal Geospatial Platform](https://www.nrcan.gc.ca/science-data/science-research/earth-sciences/geomatics/canadas-spatial-data-infrastruct/geospatial-communities-canadian/federal-geospatial-platform/11031)

## Data Creation and Manipulation

### Desktop Software
- [Esri proprietary software (ArcMap, ArcPro, ArcEnterprise, ArcOnline)](https://www.esri.com/en-us/home) can be used to manage, analyze, and visualize geospatial data. ArcPro is currently available to download in the department, and ArcEnterprise and ArcOnline will become more accessible to the department once deployed
- [QGIS](https://qgis.org/en/site/) is an open-source graphical software that is most similar to ArcMap and ArcPro. It is used to manage, analyze, and visualize spatial data. QGIS uses GDAL and you can use various open source extensions to conduct specific analyses or visualizations

#### Open Source Programming Libraries
- [Geospatial Data Abstraction Library (GDAL)](https://gdal.org/) is an open-source library for managing geospatial data
- D3.js is an open-source library for visualizing data
- geojson.io allows you to edit GeoJSONs easily
- Mapshaper
- minjur is an open-source library for managing OSM data
- osmosis is an open-source library for managing OSM data

## Spatial Data Storage

## Geo Visualizations

- Leaflet is an open-source JS library to develop interactive maps
Mapbox Studio is an open-source graphical interface for designing map layers as well as developing data-driven styling
Mapbox GL JS is an open-source library for developing interactive web maps
Mapbox Cartogram is an open-source tool to help design a map layer based on a reference image
osm2geojson is an open-source library for converting OSM data to GeoJSON(s)
PostgreSQL / PostGIS is an open-source library to store, manage, and visualize geospatial data. PostGIS has spatial index which can decrease computational time for analysis.

### Web
- [geojson.io]()
- [mapshaper]()
