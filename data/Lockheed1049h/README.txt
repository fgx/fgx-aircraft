Lockheed Super Constellation 1049H
----------------------------------

The Lockheed 1049H is a passenger/freight convertible version of the famed Lockheed 1049G. 53 were built between 1957-1958. The 1049H can be converted between configurations in just a few hours. Perhaps the best example of a surviving 1049H is the "Star of America", the "Save A Connie" Lockheed Super Constellation of the Airline History Museum at Kansas City. Though sometimes listed as a 1049G, it is actually a 1049H converted to passenger operations. You can clearly see the cargo door openings in photos of this aircraft. My model was not made to represent a particular 1049H aircraft, but rather a class of multi-purpose Connie's surviving in that role through the 70's.

The 1049H for Flightgear began life as my attempt to bring custom 3D instruments and external lights to the pre-existing older 1049G model for Flightgear. I toyed around with the idea of rebuilding the 1049G to update its appearance, but ran into problems with lack of accurate dimension information. In late summer of 2008, I stumbled on a project blog of a Swiss gentleman in the process of restoring an actual Connie cockpit, salvaged from a plane in the Caribbean which was about to be scrapped. His restoration work was stunning, and after contacting him he kindly began feeding me lots of good information. At that point I was able to build up a reasonably accurate and sometimes precise model of a real Connie cockpit, and as my modeling ability caught up I progressed to building the entire aircraft from scratch.

The 1049H still borrows much of the Flight Dynamics Model from the 1049G, and it owes a great debt to the authors of the 1049G for inspiration. All 3D models and nearly all graphics are original and built by me. The very small percentage of non-original graphics come from other Flightgear models or free public sources. My tools have been Photoshop, Inkscape, Blender, and a good-ol' text editor. My sources have been a real Connie cockpit, countless images from various sites and individuals, the 1049 maintenance manual, portions of a flight manual, portions of various other documents, and anything else I could get my hands on.

This model features the optional longer weather radar nose, though weather radar is not yet implemented. It currently does not use the optional wing-tip fuel tanks, but the new fuel system is built to accomodate these tanks so they can be easily added as a variant at a later date. It's trivial to add the tanks to the simulation.

This simulation was created using publicly available information. It contains no proprietary or restricted data, is not endorsed by any manufacturer, and is meant for entertainment purposes only. This model is being distributed under the GNU GENERAL PUBLIC LICENSE Version 2. If you like something, grab it and use it.

-Gary R. Neely "Buckaroo"


The Lockheed 1049H For Flightgear Guide
---------------------------------------

Please visit the model's home site and download the full PDF guide "The Lockheed 1049H For Flightgear":
 
http://ltts.crlt.indiana.edu/grn/flightgear/


Starting The Engines
--------------------

Above the pilot's seats you'll find the panel with the magneto switches. Engage the magnetos for the engines you wish to start by setting the switches to "Both". Switch seats to the flight engineer's station. From the engineer's station, locate the "MJB No. 1" panel to the upper left. Turn on the ship's battery or ground cart battery. Turn on all generator switches. Below that panel, find the "MJB No. 2" panel. Locate the "Engine Starter Select" switch and set that to the engine you want to start. A light should illuminate nearby, indicating that the starter is hot. Next, you would likely "Prime" a cold engine, but that button currently does nothing. Lastly press "Start" and watch your gauges for the engine to catch. Repeat for all 4 engines and you're ready to go. For more information, consult the manual at the above site.


Cockpit Space
-------------

In the current cockpit, you'll notice a relatively large space behind the captain's seat. In real Connies, this is typically occupied by a jump seat and a large rack of electronic equipment, which I have modeled in simplified detail. Much of the supporting electrical equipment for the various flight instruments can be found there, including the stuff that powers the weather radar. In Connie's heyday, the jumpseat was the radio operator's position and there was much more electrical gadgetry there, so much that it reequired special cooling air ducts to help keep all those hot tubes from driving everyone out of the cockpit.


Instrument Positions
--------------------

Real Connie cockpits, both period aircraft and late-surviving aircraft, differ widely in cockpit panel configurations. The only things that are relatively consistent are the middle flight panel (forward of the pedestal) and the engineer's main instrument display. Pilot and co-pilot panels are wildcards. As such, my standard flight display is loosely based on the latest shown in the maintenance manual, common layouts I've seen, and what I personally prefer.

Note that the little instrument to the left of the clock is control position indicator. It is not a real Connie instrument, but a modified version of the trim indicator to help keyboard flyers like me. Feel free to hunt it down in the Models/Lockheed1049h_Instruments.xml file and remove it.


The Bendix J-8 Attitude Indicator
---------------------------------

The j-8 was common in the 50's for both commercial and military aircraft, though many pilots weren't fond of it. I like its distinctive appearance, like an eyeball staring back at me. If you hate it, I've provided a more modern-style alternative AI that can be seen on the copilot side. To use it on the pilot panel, just locate the 'Lockheed1049h_Instruments.xml' file, find the AI section, and replace 'ai_j8' with 'ai'.


The Sperry Zero Reader
----------------------

This is the red AI-like instrument visible in the pilot's view. This instrument has been called the original flight director and many pilots preferred it to the more visually complex inverted V instrument that was also common to the period. The Zero Reader is not completely functional at this time. Currently it works only for ILF glide path readings using NAV1/NAV2, but eventually it will be capable of indicating a flight path based on VOR/ADF bearings and altitude/course settings.


Prop Reversing
--------------

To engage propeller reversing, first unlock the lock-out using the ctrl-L toggle. You'll see a lever on the pedestal move aft. When ready to engage reverse pitch, use the ctrl-B toggle. You'll see the pedestal throttle levers change, and the amber lights on the center main flight panel will come on.


Fuel Management
---------------

The 1049H fuel system accurately models the system of tanks and valves used in this series of aircraft. A real Constellation engineer does a lot of work monitoring and managing fuel sources. As a beginner with the 1049H you don't have to worry much about this. The default fuel settings are such that all tanks feed all engines and you have a sufficient fuel load for most regional flying.

More realistic loads and settings require much more management. Four fuel configurations are provided, accessible via the ctrl-I menu: casual flying, max takeoff, typical landing, and empty. See the Fuel HOWTO included with your 1049H for more information on managing your fuel and configuring your own custom fuel loads.

Note that if you do somehow get in trouble with fuel and need more while on the wing, you can click on the fuel gauge for a given tank to increase/decrease the fuel levels in that tank. Turn on hotspots (ctrl-c) to see these clickable areas.


Lights
------

The 1049H external light system works over Multiplayer (MP). In other words, if you turn on your landing lights in MP, others with the 1049H model will see your lights. To the best of my knowledge, the 1049H is the first aircraft in Flightgear to feature lights over MP. (Woohoo, but this also means it's also likely using the most dated method of doing it by the time you're reading this.)

Note that the landing lights are normally recessed into the underside of the wings. You must extend your landing lights if you want them to display properly.

The cabin lights dial on the pilot's left-hand panel is a cheat-- this doesn't really exist. Its location is often occupied by the windshield wiper switch. But I needed a handy way to easily control the simulated cabin lights. For this 1049H, the (inoperative) windshield wiper switch can be found on the pedestal between pilot and copilot.

All panel light switches control all cockpit instrument light levels. In reality, a given panel light switch controls only the local panel light levels. Note that in the real aircraft the main instrument panel is lit from lights and control switches mounted on the underside of the arch hood.


Livery
------

The default livery represents Eastern's colorful "Great Silver Fleet" livery of the mid to late 50's, possibly surviving in some aircraft as late as 1963. I have not identified pictures of a 1049H with this livery but I have seen pics of 1049H's with a later (and less interesting) Eastern livery. I do have a picture of what is probably a 1049G in this livery, and it is not unreasonable that an Eastern 1049H did possess this livery.

A kit for livery-makers is available at the 1049H's home site: http://ltts.crlt.indiana.edu/grn/flightgear/


Fuzzy Dice
----------

Fuzzy Dice? Yes indeed. That was a special request, and I've grown rather used to seeing them swaying there. They are, however, easily removed by going into the file Models/Lochheed1049h_Instruments.xml and removing the reference that imports the dice model. But consider how you'd be removing one of the safety features of this plane: in a pinch, the dice serve as a poor-man's Attitude Indicator.


Known problems and to-do's
--------------------------

- Cargo/passenger doors. Lack of these is somewhat embarrassing, since the cargo doors are the distinguishing feature of the 1049H, but my focus has been cockpit and instruments. 
- Prop feathering and pitch animations are not yet implemented.
- A few cockpit panels, instruments and switches are still missing or are temporary. Most of these are not essential to flight, such as the sta 260 panel on the aft cockpit wall between the crew door and the cabin door and dealing with environmental and fire extinguishing controls. At some point I may get to these, but they won't affect flight.
- An optional engine failure system is planned, for failing an engine when certain parameters are exceeded. The prototype for this exists in my Grumman Goose model.
- An optional wing-tip tank configuration is planned.
- Cowl flaps are modeled but animations disabled until appropriate engineer controls are modeled. There really is no point to cowl flaps until a way can be found to influence engine head cooling. Their drag can be implemented, but without the cooling properties they're just speed brakes.
- The propeller governor system isn't yet functional, but this and prop syncing is being planned with the help of others.


Acknowledgements
----------------

I would like to thank the builders of the Flightgear 1049G Constellation, for their work pointed the way. I would also like to thank the other Flightgear aircraft developers, particularly the work of Syd Adams, Lee Elliott, Detlef Faber, Heiko Schulz, Gerard Robin and Melchior Franz for study of their work and the work of other fine developers taught me much and set my standards, even if I can't yet meet them.

Christian Müller graciously provided me with countless photos and other information from his excellent and very real 1049 cockpit. Christian has actually flown in the Breitling Connie. I can definitely say that without him this project would not have gotten far off the ground.

The Airline History Museum in Kansas City Missouri has graciously allowed Wolfram Gottfried to photograph the cockpit of their Connie "Star of America", and has offered to answer specific questions, all of which will result in improved fidelity for the model. Please visit their site at http://www.ahmhangar.com

Wolfram Gottfried "Yakko" has provided unflagging and tireless support in helping me resolve issues with the project, research the aircraft, test the model, tweak the Wright Cyclone FDM, help perfect navigation and engine instruments, tweaked the engine sounds, and kept my morale up when it was wavering. I do believe that without Yakko this project would have floundered.

Alvaro Castañeda Mendoza "Tuxo" provided hours of help and encouragement on this project and helped me get through quite a few problems. I am very grateful.

Peter Brown "Farmboy" very kindly provided his help in flight-testing and debugging problems, updates to the sound system, and constructed the engine smoke effects.
 
Frank M. Göldner contributed the Lufthansa livery.

Brett "Gooneybird" Harrison and Durk Talsma contributed the KLM livery.

I would like to thank everyone else who has followed this project and provided support and encouragement.

---
Gary R. Neely "Buckaroo"
Dec 2010
grneely@gmail.com

