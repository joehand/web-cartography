# Weekly Schedule Details

## Week #1: GIS Fundamentals

Introduce students to the concepts of Geographic Information Systems, brief history of maps, and why we need web mapping. Get introduced to the leaflet API, learn about other ways to use GIS data.

### Competencies:

* Understand about how spatial data is produced, especially in government.
* Understand how the City of Portland distributes spatial data
* Create a map with Leaflet (*project*)
* Learn about desktop GIS applications, when they're useful (*bonus project*)

### Monday

* Introductions
* Presentation: history of GIS
* Discussion: use of maps in our lives
* Homework: 
    * basic leaflet map
    * install QGIS
    * (Reading?)

### Wednesday

* Group Workshop: desktop GIS, python (?), other GIS uses:
    * make choropleth with Portland data
    * convert shapefile to geojson
* Pairing project: leaflet + geojson
    * create map with Portland geojson data
* Homework:
    * Choropleth w/ Portland shapes (bonus: Interactive?)
    * (Reading?)

## Week #2: Web Map Fundamentals, Data Exploration

History of web maps and how they evolved to the maps we have now. Tiles, ajax, slippy maps.

### Monday

* Discussion: Map Critique + Review homework
* Presentation: web mapping fundamentals
* ?
* Homework:
    * leaflet geojson w/ ajax
    * video (?) https://vimeo.com/106112939

### Wednesday

* Group workshop:
    * Demo web fundamentals with leaflet: changing tiles, zoom stuff, etc.
* Pairing: 
    * Modifying map state with timing/interaction
* Homework:
    * Exploring plugins: ideas (heatmap, marker clustering)
    * cool thing: tour of portland scratch map - how to connect this idea to portland civic ? (https://github.com/JamesMilnerUK/scratchmap/blob/gh-pages/map.html)

## Week #3: Spatial Data + Vector Tiles

Learn about spatial data formats. mapbox-gl

### Monday:

* Discussion: review homework, map critiques 
* Presentation: intro to spatial data, geojson
* Homework:
    - sign up for mapbox
    - make a cool map style! use in mapbox-gl
    - Reading(?)

### Wednesday

* Presentation: vector tiles vs raster
* Pairing/homework:
    - Live updating geojson data (bike share, trimet?) (https://www.mapbox.com/mapbox-gl-js/example/live-update-feature/) (https://www.mapbox.com/mapbox-gl-js/example/live-geojson/)
    - choropleth drill down (https://www.mapbox.com/mapbox-gl-js/example/updating-choropleth/)
    - Reading(?)

## Week #4: Spatial data processing

introduction to geojson, command line data processing tools.

### Monday

* discussion: map critique, homework review
* Presentation: intro to ogr2 etc., spatial data processing ideas, topojson
* homework
    - reading https://macwright.org/2015/03/23/geojson-second-bite.html, https://macwright.org/2016/06/05/falsehoods-developers-believe-about-geojson.html

### Wednesday

* Group workshop: d3 command line processing
* Pairing: o/ with other data
* Homework:
    - spatial data processing on other data?

## Week #5: mappin with d3

mapping with d3

### Monday

* discussion
* presentation: d3 vs tile mapping
* homework:

### Wednesday

* voronoi d3/leaflet https://chriszetter.com/blog/2014/06/15/building-a-voronoi-map-with-d3-and-leaflet/
