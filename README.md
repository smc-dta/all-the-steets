# All the streets of a America

![](example.png)

Generate your own map of every street in America.

First run:

    npm install

You might have install cairo, if you haven't already. See the instructions on [node-canvas](https://github.com/Automattic/node-canvas) project page.


You might also need to install the `ogr2gr2` and `topojson` command line utilities. (The ogr2ogr is included in the gdal package.) Checkout Mike Bostock's [Let's make a map](http://bost.ocks.org/mike/map/) for more details.

    brew install gdal

    npm install -g topojson


Next, run

    node download.js

This will download the data for the [US Census](http://www2.census.gov/geo/tiger/TIGER2014/ROADS/) website and run ogr2gr as well as convert the geojson files to topojson. Next, Grab coffee. It's going to take a while (1-2 hours).


Now run you can

    node draw.js

Which will generate the image to `out/out.png`. Feel free to modify the `draw.js` script to your liking.
