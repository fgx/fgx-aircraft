Read this First:
After unzipping this ZIP file into your $FGBASE/data/Aircraft directory,

Choose your aircraft:
 start Flightgear with the following parameter:

If you are running the newest version of FlightGear, 
  version 2.0, 1.9 or cvs built with OpenSceneGraph,
    --aircraft=bluebird

If you are running FlightGear version 1.0 (with Plib)
  or if you are running FlightGear version 0.9.10
  and for some reason are unable to upgrade, then look
  for the legacy version 8.81 at http://seahorseCorral.org

-------------------------------------------------

After the simulator starts up, your power is on, the engines 
  are on standby, and ready to throttle up.
  To hover up, press [Home] to spin up the counter-grav hover fans,
  or drag the middle mouse button in pointer mode.

Press [?] for help with keyboard shortcuts specific to this model.
For more basic help, press [F10] to toggle the menu bar, 
  then select Help, and Basic Keys.

If you want the multiplayer model for OSG, 
unzip the (separate) bluebird-ai.zip file into your $FGBASE/data directory.
It will extract into the AI/Aircraft directory.

-------------------------------------------------

When editing an animation for Waldo Walker,
 please remember the following tips:
 After entering a text box, press Enter
 After changing anything, Remember to press Save before leaving 
   the dialog, or the current position ( like pressing [+] or [-] )

-------------------------------------------------
2009 by Stewart Andreason for FlightGear

Send Suggestions? Comments? Problems? or Encouragement to:
  sandreas41 <at> gmail <dot> com
Stay current with latest version. This model came from: 
  http://seahorseCorral.org/flightgear_aircraft.html

Highlights in this model:
  Hover capable
    Counter-Grav or Turbo-Fan (you imagine the technology)
  Capable of Orbital velocities
    (but remember FlightGear is for flying near the ground, not in space)  :)
    Trans-oceanic flights in minutes.
  Variable Interior lighting at night.
  Digital cockpit.
  Lots of buttons and lights in cockpit.
  Varying flight modes with different combinations of engines when
    one or the other is turned off.
  Crashing can degrade performance until you blow the nacelles off.
    New venting and sparking effects.
    After the 3rd crash, you will have to make repairs (and reset)
  Large cockpit with unobstructed view.
  Landing Gear has 4 deployment modes.
  Open hatches respond to gear height.
  Landing lights and nav lights have "On at Dusk" and "Stay On" modes.
  Windows can be polarized.
  Plenty of glows and sound effects.
  Customizable color and/or textures for most surfaces.
    To create new colors or apply images to the fuselage,
    Create a new file in the Models/Liveries directory by copying an existing one,
     then change the colors as desired.
    See the livery-template.rgb file in the Models/Textures directory, edit with
     an editor capable of writing SGI and RGB files (like GIMP)
     Draw in the non-black areas, following the dots that correspond to the 
     fuselage surface, then save as a new filename.RGB

  Capable of walking around cockpit and around aircraft,
   out the doors or hatches to ground, 
   or jump when airborne like a sky diver.
  Free fall with or without a parachute at terminal velocity.
  Cockpit display screens ready to be filled with multiplayer, weather radar,
   gps maps, etc.
  Walker can walk out and in through the hatches,
   around on the ground, 
   jump out and parachute to ground, 
   or climb non-vertical walls.
  Multiplayer
  Walker animations.

Current development level is: Early-Production
 All significant bugs within my model are (believed to be) fixed.
 Some further development is always likely or unavoidable.

 Wish list:  Synchronize door sounds when gear is not down fully.
              sound.xml seems limited in select and property conditions.

 Known bugs that seem to be unique to the ufo flight model:
             Looped sounds stay off until forward trottle.
               Have made a workaround to get rumble sound on at startup with hover.
             Flight controls (throttle, elevator, roll)
               still work after a power shutdown.
             Standard Attitude indicator does not work. 
               ufo model writes "power off" numbers to standard location.
                 workaround is in place, see ufo-ai.xml
             Can not land or drive on hills. Flight attitude is hard linked to 
               joystick controls.

-------------------------------------------------
Credits:
  Some sound files are by Michelle Pay (aerotro)
    altitude-1.wav
    altitude-0-loop.wav
  Waldo Walker is by Detlef Faber
-------------------------------------------------

 ___________ This model is released under the terms of the GPLv2 ___________
 #    This program is free software; you can redistribute it and/or modify  #
 #    it under the terms of the GNU General Public License as published by  #
 #    the Free Software Foundation; either version 2 of the License, or     #
 #    (at your option) any later version.                                   #
 #                                                                          #
 #    This program is distributed in the hope that it will be useful,       #
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of        #
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the         #
 #    GNU General Public License for more details.                          #
 ---------------------------------------------------------------------------
