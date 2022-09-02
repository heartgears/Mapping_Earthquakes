# Mapping_Earthquakes
![earthquake_banner](https://thumbs.dreamstime.com/b/vector-illustration-earthquake-curve-wave-earth-crack-red-background-166578158.jpg)

## Purpose
The purpose of this project is to visually show the differences between the magnitudes of earthquakes all over the world for the last seven days.

![Mapping_Earthquakes](https://github.com/heartgears/Mapping_Earthquakes/blob/main/Mapping_Earthquakes.png)

## Technology and Requirements

This project requires a [URL for GeoJSON earthquake data from the USGS website](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson) to retrieve geographical coordinates and the magnitudes of earthquakes for the last seven days. This data is then added to a map using the JavaScript and the D3.js library. This is done using the Leaflet library to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data.

The following technologies were utilized:
* Data Sources: 'tectonic_plate_starter_logic.js', 'tectonic_plate_starter_logic.js', 'tectonic_plate_starter_logic.js' and 'index.html'
* Data Tools: JavaScript, JSON, GeoJSON and IO (Web Server)
* Softwares: ES6+, ECMAScript and Visual Studio Code 1.50.0

## Results
### 1. Adding the Tectonic Plate Data
* The tectonic plate data is added as a second layer group
* The tectonic plate data is added to the overlay object
* The tectonic plate data is passed to the 'geoJSON()' layer
* The 'geoJSON()' layer adds color and width to the tectonic plate lines
* The tectonic layer group variable is added to the map

### 2. Adding the Major Earthquake Data
* The major earthquake data is added as a third layer group.
* The major earthquake data is added to the overlay object.

The d3.json() callback does the following:
* Sets the color and diameter of each earthquake.
* The major earthquake data is passed to the geoJSON() layer.
* The geoJSON() layer creates a circle for each major earthquake, and adds a popup for each circle to display the magnitude and location of the earthquake
* The major earthquake layer group variable is added to the map

### 3. Additional Map Tiling
* A third map tile layer is created, the dark layer.
* This third map is added to the overlay object.
* All the earthquake data and tectonic plate data are displayed on the all maps of the webpage.
