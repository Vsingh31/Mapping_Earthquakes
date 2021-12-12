# Mapping_Earthquakes
## Project Overview
The objective of this project is to gather earthquake GeoJSON data from the USGS API, create and explore interactive maps of earthquakes around the world.
The earthquake data is represented on the maps in relation to the tectonic plates’ location on the earth, and according to each event's magnitude.
Maps allow us to explore, understand, and make decisions about our world. In this repository we will use javascript (GeoJSON) to create interactive maps to visualize earthquake data. GeoJSON data can be found in many apps that have a map feature such as ride-sharing, navigation, and food and package delivery services. Even location services on smart phones use GeoSJON format.

### Resources
* Data Source: [Earthquakes GeoJSON](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson), [Earthquakes above 4.5mag GeoJSON](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson) ,[Tectonic Plate GeoJSON](https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json) 
* Software: HTML/CSS, JavaScript, Visual Studio Code, Leaflet 1.7.1, D3.js 6.2.0

#### Results
Each earthquake is visually represented by a circle and different colors according to their magnitude, where a higher magnitude will have a larger diameter and will be darker in color. In addition, each earthquake has a popup marker that, when clicked, shows the magnitude of the earthquake and the location of the earthquake. The map has three views:

* Street View
* Satellite View
* Dark View

The viewer can also toggle between three layers to filter the data. These layers include:

* All Earthquakes
* Tectonic Plates
* Major Earthquakes (greater than 4.5 magnitude)


![earthquake](https://user-images.githubusercontent.com/90277142/145723225-d81ce45d-1530-45e8-b5a8-7f5a216cf2f5.png)

![Satelliteview](https://user-images.githubusercontent.com/90277142/145723234-d778e9a7-1cab-47b1-b267-9838ecb57655.png)

![Darktile](https://user-images.githubusercontent.com/90277142/145723240-235eeeb3-fc44-4eaa-9b70-cde33d46f313.png)


#### Summary
To create the maps we used the JavaScript and the D3.js library to retrieve the coordinates and magnitudes of the earthquakes from the GeoJSON data.

Calling the API's allowed us to traverse and retrieve GeoJSON earthquake data and tectonic plate data in order to populate a map. We then used the Leaflet library to plot the data on a Mapbox map through an API request and create interactivity for the earthquake data. The viewer can toggle between different layers to view either all earthquakes, only major earthquakes (over 4.5 magnitude), and the earth's tectonic plates.
