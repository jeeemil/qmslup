# Visualizing City Bike Data in Helsinki and Espoo

This repository is home to a jupyter notebook that can help you extract data from the Shared Bicycle System in Helsinki and Espoo. For more information about the Shared Bicycle system visit [the homepage](https://kaupunkipyorat.hsl.fi/en). The main purpose is to get some useful spatial files as output, so that they can be used in a software like QGIS. A temporal factor is added, by dividing the data into day and night time data sets.

### The things you can get from this repo is:
* CSV-files with the night or day time trips spearately for a certain month. 
* A geopackage with all bike trips from a certain month, with the departure or return station geometry. You get the data for day and night trips separately.
* A geopackage with the averaged data for each bike station for either the departed or returned trips. This data includes the average duration in minutes, average distance covered and the number of trips. This data is also separated between day and night trips.
* A geopackage with the euclidean lines between departure and return station for either day or night time data.

### Python packages used:
* [geopandas](http://geopandas.org/) 0.8.1
* [pandas](https://pandas.pydata.org/) 1.1.3
* [shapely](https://pypi.org/project/Shapely/) 1.7.1
* [requests](https://requests.readthedocs.io/en/master/) 2.25.0

This repository was developed during the course GEOG-326, Quantitative methods for sustainable land use planning (QMSLUP) I: Accessibility and mobility analyses, at the University of Helsinki.

### Data

* [Data over Shared Bicycle Trips](https://classic.hsl.fi/en/opendata)
* [Data over Shared Bicycle Stations](https://public-transport-hslhrt.opendata.arcgis.com/datasets/helsingin-ja-espoon-kaupunkipy%C3%B6r%C3%A4asemat/data)

### Example of what the output can be used for

This is an example map of what the data can include. The ouput style has been modified with QGIS.

![Shared bike rides during the night in June 2019](https://github.com/jeeemil/qmslup/blob/main/example_map.png)
