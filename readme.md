FGx AirCraft
============

# Preamble:

Theo pointed the way to load Three.js json models (3js) into a global scene. The initial, very manual way to get this 3js was to load the flightgear ac3d (.ac) model into blender, then export it as dae, then load that dae and export it as 3js. It works, but is quite cumbersome. And the blender UI take some understanding...

I had already started experiments with some ac3d2gl sources. That is load an ac3d model file and render it in GL. And the source of these experiments are in my fgtool repo - http://gitorious.org/fgtools/ac3d2gl - but this only started to identify the problems... While MOST ac3d *.ac files list all faces with 3 (or 4) vertices, some like say the fg 707.ac have faces with 64 vertices! How to render these in GL?

My next attempt was in a project called ac2glview ( TODO - http://gitorious.org/fgtools/ac2glview ). Here I developed an ac3d_browser2 program which loads an ac3d *.ac file, shows a GL view, and lists the components. Each component can be expanded in the list, selected, and an attempt is made to give a GL view of that single item. And, if not needed in the final model, like light cones, wheels, other artifacts, they can be deleted, and a cleaned .ac files written.

To this program I also added the ability to 'export' the model directly to 3js, and while this works well for a large number of model files, it fails when any of the faces contains more than 3 or 4 vertices. Lots of effort was put into solving this, but could not get it right...

I messed around with some other sources, like mview, which supports a considerable list of 3D formats - PMesh, GTS, OFF/COFF, ply, VRML 1/2, shallo?, vtk and obj. But on reviewing most of these again all faces have 3 vertices, and in some rare cases 4. Never values like 64!

This track led me deeper into the geomview (OFF/COFF) source, but while it compiles and runs well in Ubuntu linux, it proved too difficult to compile in Windows. It is too mixed up with Motif and X11!

By chance I ran across assimp ( http://assimp.sourceforge.net/ ). To quote from their websit "Open Asset Import Library (short name: Assimp) is a portable Open Source library to import various well-known 3D model formats in a uniform manner. The most recent version also knows how to export 3d files and is therefore suitable as a general-purpose 3D model converter.". And added to that it supports 'scripting' of the load, post processing and exporting...

Naturally the loading included ac3d *.ac model files, but it only exported dae, obj, stl and ply. But I knew one of these must have the same constraints as 3js, namely ALL faces must be described as 'triangles', that is sets of 3 vertices. So I copied the 'obj' exporter, and changed the code to output 3js, AND IT WORKED ;=))

So then we have the action chain -
load the model into ac3d_browser2
review and delete unwanted components if any
write a modified new *.ac file
load that ac file into assimp_viewer
exort as 3js
And bingo we have the desired web 3js model file. Some of this process is aided by the fact that both programs, ac3d_browser2 and assimp. On exit ac3d_browser2 will generate a 'script' to repeat the process, whihc includes a script to run assimp and export the 3js. Namely the last two steps listed above.

So excluding the manual review step 2, I was able to create a big list of FG model ac file - aclist-ac.txt - and use a batch file to process them ALL. This gave me a set of 435 3js files to load and view. They range in size from the small 5,310 byte paperairplane.js, to the massive 73,155,108 byte Vostok-1-TDU.js

# Viewer:

One-by-one - Load an view each of the 435 models separately. It sports a [next] and [back] links, and a small GUI to select any of the 435 models, with some display options.

Load a set - This loads a set of about 20 planes into the scene

Old 1x1 - Early version of the one by one viewing

ac-01.zip - A zip file containing the 435 3js model files (190MB)

And just to be sure I got everything globe-02.zip is the entire contents of this 'globe' folders, including 4 sub-directories, only excluding the above zip, which is effectively the ac folder contents, so that folder is also excluded...

That ac folder contains 436 <model>.js files, 414 of which are used in the above 1x1 display (load-one2.html). It als