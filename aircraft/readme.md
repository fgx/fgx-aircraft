FGx Aircraft Read Me
====================

This directory contains the data files for 430+ aircraft imprted from FlightGear files and converted to Three.js JSON format.
Every aircrafy has its own directory which apart from the JSON data file contains read me, license, thumbbnails, splash screen 
and any other text files found in the original source code directories.

This is the prime reposotory for aircraft data for use by FGx Globe and other apps in the pipeline.

There is a rudimentary aircraft viewer: [FGx Aircraft Viewer]( ../aircraft-viewer/r2/aircraft-viewer.html )
 

### Issues
* Dropdown list fails completely in Firefox - though next and previous buttons both work.

### Source Code
[github.com/fgx/fgx-aircraft](https://github.com/fgx/fgx-aircraft/tree/gh-pages/ )

### Aircraft Road Map
* Priority: complete movement of each aircraft into appropriate directory
* Agree a naming convention for aircraft files and their folders. See below for thoughts.

* Meld duplicate vertices and redefine normals for each aircraft using Blender. 
	This much reduces file sizes and de-facets the skins of the aircraft
	* Perhaps can build Python utility to help
* Ascertain original scale and rescale planes so they are all at the same scale
* Point all planes in the same direction
* Agree a suitable base point (the nose or most forward point of the body of an aircraft?) and apply to each aircraft
* Build a table that includes relevant data for each plane for each plane with 
	* link to source in fgdata on Gitorious
	* link to entry on Wikipedia
	* unit system used to create the model (feet, inches, cm, mm etc)
	* Whether it has a thumbnail*
	* whether data has been smoothed or not

* Investigate adding livery bitmaps


### Aircraft Files and Folders Naming Convention << Request for Comments

The names of aircraft files and folders as supplied by FlightGear appear to follow no particular guidelines. 
This makes it difficult to know which plane is in which folder.
This section begins to outline suggestions for a naming convention.


#### Follow Wikipedia

* Examples:
	from: 14bis
	to: Santos-Dumont_14-bis
	from: T-4
	to: Kawasaki_T-4  << and not http://en.wikipedia.org/wiki/Sukhoi_T-4
	
* Wikipedia entries have many eyes; tend to get things properly disambiguated 

#### Normal webbish convention
* make it as easy as possible for a human to type 
* all lower case
* short as possible
* hyphens between words, no underscores 

It would be better to make it so that nobody ever feels like typing


### Tips
To create CSV file of aircraft quickly:

    dir *.js /s /b > aircraft.csv


### Copyright and License
copyright &copy; 2013 FGx authors ~ All work herein is under the [GPL 2.0 License](https://github.com/fgx/fgx-aircraft/blob/gh-pages/license.md)


### Aircraft Copyright and License
The original data for each aircraft is derived from the models obtained the 'Aircraft' directory here: https://gitorious.org/fg/fgdata/

Each model has been converted from .AC format to .JSON format with the assistance of a scheme devised by Geoff McLane as described in his [Read Me](https://github.com/fgx/fgx-aircraft/blob/gh-pages/readme-r1.md).

The directory for each model contains the read me and license for the aircraft as supplied by the original author of the model and copied here from the FG source.


### Change Log

2013-12-03 ~ Theo
* Added this Read Me
* 400+ folders added. Titles and content (thumbnails, read me, license etc) brought over from FlightGear source on Gitorious
* 300+ JSON models moved into appropriate folder
* Create directories for each plane
* Add thumbnails, license and original authors notes for each plane 
* Updated CSV file