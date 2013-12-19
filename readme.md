![FGx Logo]( http://fgx.github.io/images/fgx-cap-40x30.png) FGx Aircraft Read Me
================================================================================


Cropped `iframe` view of the FGx Aircraft Overview app:		
<iframe src="http://fgx.github.io/fgx-aircraft-overview/r4/aircraft-overview.html" width=100% height=300px>
There is an `iframe` here. It is not visible when viewed on github.com/fgx. To view, please go to fgx.github.io.
</iframe>


## Concept
The objective of this project is to make available as [Three.js JSON]( https://github.com/mrdoob/three.js/wiki/JSON-Model-format-3.1 ) files 
all the aircraft and other 3D models that are created for FlightGear.

This repository currently contains the data files for 430+ aircraft and other vehicles imported from FlightGear files and converted to Three.js JSON format.

Every aircraft has its own directory which apart from the JSON data file contains read me, license, thumbnails, splash screen 
and any other text files found in the original source code directories.

This is the prime repository for aircraft data for use by FGx Globe and other apps in the pipeline.

 
## Features
 
As Three.js JSON files, the aircraft may be easily displayed and manipulated in a browser.

Here is a typical example of the code:

[Santos-Dumont 14bis]( http://fgx.github.io/fgx-aircraft/data/14bis/14bis.js )

All the aircraft have a GPL 2 license and and may be linked to from this project.

A longer term objective might be to accept models from any source and create a virtual museum of flyable aircraft.


## Project Links

You have two ways of viewing the FGx Aircraft files:  

* Code hosted on GitHub: [fgx.github.io/fgx-aircraft]( http://fgx.github.io/fgx-aircraft/ "view the files as apps." ) <input value="<< You are now probably here." size=28 style="font:bold 12pt monospace;border-width:0;" >  
* Source code on GitHub: [github.com/fgx/fgx-aircraft]( https://github.com/fgx/fgx-aircraft/ "View the files as source code." ) <scan style=display:none ><< You are now probably here.</scan>

Latest revisions of the aircraft browser / viewers:

* [FGx Aircraft Loader]( http://fgx.github.io/fgx-aircraft-loader/load-one.html )
* [FGx Aircraft Overview]( http://fgx.github.io/fgx-aircraft-overview/latest.html )

See also the Read Me files for the browser / viewers for details on features and road maps:

* [FGx Aircraft Loader Read Me]( http://fgx.github.io/fgx-aircraft-loader/index.html )
* [FGx Aircraft Overview Read Me]( http://fgx.github.io/fgx-aircraft-overview/index.html ) 

## Issues

* <s>~~Priority: complete movement of each aircraft into appropriate directory~~</s> Fixed
* Dropdown list fails completely in FireFox - though next and previous buttons both work.
* Missing aircraft include:
	* Cessna p172 Skyhawk ~ the most popular plane ever made
	* DC-10
	* A-320 

## <a name="roadMap"></a> Aircraft Road Map

### Overview

Geoff's work and success in converting hundreds FlightGear aircraft from AC format to Three.js JSON format is quite extraordinary.

The current set of models, while fun to browse, nonetheless suffer from issues including:

* Aircraft with missing or superfluous elements
* Varying scale
* Duplicate vertices

With a bit of thought and some hours of labor it will be possible either edit the models or edit Geoff's converter
so that the models form a coherent collection and are truly usable.

Items that need attention include the following:

* Agree a naming convention for aircraft files and their folders. See below for thoughts.

* Meld duplicate vertices and redefine normals for each aircraft using Blender. 
	* This much reduces file sizes and de-facets the skins of the aircraft
	* Perhaps we can build Python utility to help
* Ascertain original scale and rescale planes so they are all at the same scale
* Point all planes in the same direction
* Agree a suitable base point (the nose or most forward point of the body of an aircraft?) and apply to each aircraft
* Build a CSV table that includes relevant data for each plane for each plane with; 
	* Link to source in fgdata on Gitorious
	* Link to entry on Wikipedia
	* Unit system used to create the model (feet, inches, cm, mm etc)
	* Whether aircraft has a thumbnail
	* Whether data has been smoothed or not and any other work-in-progress data

* Investigate adding livery bitmaps

### Action Items

* Create a CSV file. File to list every model in the FlightGear fgdata directories
* Start populating list with categories listed above, including whether models exists in FGx Aircraft
* Examine data in fgdata to determine what parameters can be inferred algorithmically including scale, units and base point.
* Decide who should write Python utility to eliminate duplicate vertices using Python - or see if Geoff's converter could be tweaked to do this.
* Ascertain which models might need work in Blender. Decide who does what.


### Aircraft Files and Folders Naming Convention << Request for Comments

The names of aircraft files and folders as supplied by FlightGear appear to follow no particular guidelines. 
This makes it difficult to know which plane is in which folder.
This section begins to outline suggestions for a naming convention.


### Follow Wikipedia Naming Convention

* Examples:
	* from: 14bis
	* to: Santos-Dumont_14-bis
	* from: T-4
	* to: Kawasaki_T-4  << and not http://en.wikipedia.org/wiki/Sukhoi_T-4
	
* Wikipedia entries have many eyes; tend to get things properly disambiguated 

### Normal Webbish Naming Convention

* make it as easy as possible for a human to type 
* all lower case
* short as possible
* hyphens between words, no underscores 

It would be better to make it so that nobody ever feels like typing


## Tips
To create CSV file of aircraft quickly:

    dir *.js /s /b > aircraft.csv
	
	
## System Requirements
In order to view the files on this site you will need a device and browser that provides good support for [WebGL](http://get.webgl.org/)
WebGL is the JavaScript API for rendering interactive 3D graphics and 2D graphics within any compatible web browser without the use of plug-ins. 

Generally this means a computer with an Intel Core i5 processor or better with an external GPU such as one made by Nvidia. 
Successful use of the apps on a phone or tablet is highly unlikely. 
A mouse or other pointing device with a scroll wheel is also highly recommended so that you can zoom, pant and rotate in 3D.

The apps here may work in the Google Chrome or Mozilla FireFox browser, but most likely will not work with Apple Safari or Microsoft Internet Explorer. 
The apps here are currently being built and tested with the Google Chrome browser. 
Bugs on browsers other than Chrome need not be reported until such time as the work settles down and an effort to support more browsers is initiated.


## Copyright and License
copyright &copy; 2013 FGx authors ~ All work herein is under the [GPL 2.0 License](https://github.com/fgx/fgx-aircraft/blob/gh-pages/license.md)


## Aircraft Copyright and License
This repository is at an early and volatile stage. Not all licensing requirements may have been fully met let alone identified. It is the intension of the authors to play fair and all such requirements will either be met or the feature in question will turned off.

The original data for each aircraft is derived from the models obtained the 'Aircraft' directory here: https://gitorious.org/fg/fgdata/

Each model has been converted from .AC format to .JSON format with the assistance of a scheme devised by Geoff McLane as described in his [Read Me](https://github.com/fgx/fgx-aircraft/blob/gh-pages/readme-r1.md).

The directory for each model contains the read me and license for the aircraft as supplied by the original author of the model and copied here from the FG source.



## Change Log

2013-12-18 ~ Theo

* Combined the two read me files
* Expanded read me file
* Fixed Wright Flyer being in wrong directory

2013-12-06 ~ Theo

* seymour in folder
* splash.txt created in aircrat dir
* aircraft.txt created in aircrat dir

2013-12-05 ~ Theo

* Geoff's and Theo's viewer move to new repos
* Files cleaned here
* Directory 'aircraft' renamed to 'data' because './aircraft/aircraft' seemed lame

2013-12-05 ~ Theo

* Completed moving aircraft .JS files to their proper folders


2013-12-04 ~ Theo

* Added iframe view of viewer and other text to main read me.

2013-12-03 ~ Theo

* Add Aircraft Read Me
* Add Aircraft Viewer Read me

2013-12-04 ~ Theo

* Moved a dozen or so data files into their apprprate directories
 

2013-12-03 ~ Theo

* Added this Read Me
* 400+ folders added. Titles and content (thumbnails, read me, license etc) brought over from FlightGear source on Gitorious
* 300+ JSON models moved into appropriate folder
* Create directories for each plane
* Add thumbnails, license and original authors notes for each plane 
* Updated CSV file

2013-12-02 ~ Theo

* Viewer renamed to 'FGx Aircraft Viewer'
* Viewer moved to its own folder
* Viewer loads aircraft via dropdown list
* Info box added
* Code clean up
* Geoff r1 text moved to separate read me.

2013-11-18? ~ Theo

* R1 folders and files added

