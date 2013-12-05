Lockheed 1049 real data
=======================
Weight : max takeoff 120000 lb, max landing 98500 lb, maximum without fuel 93500 lb (A).

Vne (never exceed)           : 293 kt until 11000 ft; then - 11 kt / 2000 ft (A).
Vno (normal operation)       : 260 kt until 11000 ft, then - 9 kt / 2000 ft (A).
Vf (takeoff flaps 60%)       : 184 kt (A).
Va (maneuvring)              : 180 kt (A).
Vlo (landing gear operation) : 165 kt (A).
Vle (landing gear extension) : 165 kt (A).
Vf (approach flaps 66%)      : 161 kt (A).
Vf (80%)                     : 153 kt (A).
Vf (landing flaps 100%)      : 148 kt (A).

Engine limits : - takeoff (2.75 minutes) : sea level,   54.5 inhg 2900 rpm;
                                           at 4500 ft,  52.5 inhg 2900 rpm (A).
                - maximum continuous :     sea level,   48.0 inhg 2600 rpm;
                                           at 5300 ft,  46.0 inhg 2600 rpm;
                                           at 10800 ft, 47.5 inhg 2600 rpm;
                                           at 16000 ft, 46.0 inhg 2600 rpm (A).


Climb rate : 1125 ft/min (F).
Ceiling : 25000 ft (A).
Range (max payload) : 1049 : 1890 NM (E).


Comparison with other 1049s
===========================
Cruise  : 6000 m [19700 ft] (F).
Ceiling : - 25000 ft (B)(C).
          - 23200 ft (D).
          - 8500 m [27900 ft] (F).
Range (max payload) :
          - 1049C : 2510 NM (E).
Range (max fuel) :
          - 1049C : 4160 NM (B).
          - 3450 NM, 16.5 h maximum, 24790 l (C). 
          - 3500 NM, 14 h without reserve, 6550 US gal (D).
          - 1049C : 4760 NM (E).

The range of 1049 should be 3580 NM = 4760 x (1890 / 2510).


Lockheed 1049 ops
=================
- take-off : - flaps 1/4, 2900 RPM.
             - rotation 130 kt (full load), 120 kt (landing load) :
               raise slowly the nose until the gear lefts the ground (a little nose heavy).
             - retract gear below 165 kt.
             - retract flaps below 184 kt.
- climb    : - always above 180 kt (drag).
             - below 48 inhg and 2600 RPM (engine temperature).
             - reduce pitch to the lowest RPM (if not enough, reduce throttle),
               then reduce mixture to the highest RPM (and torque) (G).
             - decrease mixture (highest EGT) with altitude, otherwise engine stops.
- cruise   : - 220 kt at 20000 ft, 197 kt at 25000 ft (2600 RPM).
             - min mixture, min pitch (with stable RPM).
- descent  : - max pitch (i.e. lowest thrust of propeller curve).
- approach : - max pitch, level to reduce speed.
             - 10 NM at 1500 ft.
             - flaps 1/4 below 184 kt.
             - gear below 165 kt.
             - flaps 1/2 below 161 kt.
             - flaps 3/4 below 153 kt.
             - full flaps below 148 kt.
             - maintain 125 kt (landing load). 
- landing  : - 110 kt (landing load), 100 kt (empty load).


Installation
============
A mouse with 3rd (middle) button, or its emulation (left + right button), is required.

Fuel load
---------
- default is maximum landing weight, 98500 lb.
- for alternate load, press "ctrl-I f" (saved on exit in aircraft-data).

Sounds
------
See Sounds/Lockheed1049-mats-sound.xml to install Constellation sounds (recommended).

Known compatibility
-------------------
- 2.6.0 : minimum version.


Keyboard
========
- "ctrl-F" : surface control boost.
- "f"      : "f"ull cockpit (all instruments).
- "q"      : quit speed up.

Views
-----
- "ctrl-E" : "E"ngineer view.
- "ctrl-J" : Copilot view.
- "ctrl-K" : Observer view (floating).
- "ctrl-L" : Observer 2 view (floating).
- "ctrl-N" : "N"avigator view.
- "ctrl-O" : radi"O" view.
- "shift-ctrl-V" : restore view pitch.
- "shift-ctrl-X" : restore floating view.

Virtual crew
------------
- "ctrl-Z" : virtual crew.

Unchanged behaviour
-------------------
- "x / X"  : zooms in the small fonts; reset with "ctrl-X".

Same behaviour
--------------
- "S"   : swaps between Captain and Engineer 2D panels.
- "F12" : radio frequencies.
 
Improved behaviour
------------------
- "ctrl-A" : hold altitude.
- "ctrl-H" : toggle autopilot (hold heading and pitch).
- "ctrl-P" : toggle autopilot (hold heading and pitch).
- "ctrl-S" : autothrottle (virtual copilot).
- "up / down"  : increases / decreases (fast) pitch hold.
- "home / end" : increases / decreases (slow) pitch hold.
- "page up / page down" : increases / decreases copilot speed.
- "a / A"  : speeds up BOTH speed and time. Until X 10.
  Automatically resets to 1, when above 2000 ft/min.

Alternate behaviour
-------------------
- "ctrl-B" : propeller reverse (not yet implemented by FDM).
- "ctrl-I" : menu.
- "up / down"  : move floating view in length.
- "home / end" : move floating view in length (fast).
- "left / right" : move floating view in width.
- "page up / page down" : move floating view in height.


Mouse
=====

ADF
---
To update the frequency of ADF 2 :
- press "XFR" on the overhead.
- press "ctrl-R" to call the radio menu. 

When out of range, ADF needle parks at 90 degrees.

Cross-feed
----------
To feed an engine with the tanks of another engine, set fully the lever at the bottom. 

VOR
---
When out of range, VOR needle is steady (use light of deviation indicator).


Virtual copilot
===============
Virtual copilot :
- can hold throttle and follow waypoints.
- is never the pilot in command.


Consumption
===========
Cruise speed 2300 RPM (full throttle, min pitch, min mixture), for 1 engine :
- full load, 220 kt 130 gallons/h at 20000 ft, 2450 RPM (J = 1.89).
- empty load,197 kt 150 gallons/h at 25000 ft, 2450 RPM (J = 1.56).

As the real fuel is 1 US gal = 6 lb (A), multiply by 6.6 / 6 to compare with the real consumption.

All with lateral wind.
Min mixture : before engine cutoff.
Min pitch : before influence on RPM.

Example
-------
KJFK - EHAM , 3200 NM (via CYQM Moncton, CYQX Gander, EINN Shannon) :
- at 20h50 zulu (afternoon), takeoff at full load (5954 gallons), heading 85 deg.
- tail wind 270 deg 20 kt.
- cruise starts at 20000 ft, +1000 ft every 2h.
- after 10h15, lands in the morning with 400 gallons or 0h45 (135 gallons/h).

EHAM - KJFK , 3200 NM (via EINN Shannon, CYQX Gander, CYQM Moncton) :
- at 6h15 zulu (morning), takeoff at full load (5954 gallons), heading 285 deg.
- head wind 270 deg 20 kt.
- cruise starts at 20000 ft, +1000 ft every 2h.
- after 10h, cruises CYQM with 670 gallons at 515 NM from KJFK.
- after 12h, run out of fuel at 0h30 of KJFK.


JSBSim
======
- real propeller diameter (15.0 ft).
- real gear ratio 16:7.


TO DO
=====
- 3D instruments.
- scale instruments on engineer panel.

TO DO FDM
---------
- reversed propeller : ctrl-B only animates the lights and levers.


Known problems
==============
- data are not saved on reinit.

Known problems autopilot
------------------------
- toggle waypoint following (virtual copilot), only AFTER activation of route, or use "ctrl-I a".

Known problems 2.4.0 autopilot
------------------------------
- on engagement, magnetic and true heading modes bank into the opposite direction.

Known problems FDM
------------------
- cross feed emulation until speed-up X 3, when empty tank.
- at rest, idle engine (700 RPM) may yet stop by very low pressure (altimeter 29.49 inhg).
- at rest, idle engine (700 RPM) may stop by normal pressure (altimeter 29.89 inhg),
  when the RPM goes strongly below 700 RPM, by a curt throttle : visible by RPM oscillating around 700 RPM.


Secondary problems
==================

Secondary problems FDM
----------------------
- negativ oil pressure.
- cylinder head temperature too high.


References
==========
(A) http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/MainFrame?OpenFrameSet :
    (FAA certificate, 6a5 - 14 may 1952).

(B) http://cip.physik.uni-wuerzburg.de/~pschirus/aviation/flugzeuge/constellation.phtml :

(C) http://www.hars.com.au/fleet/constellation/facts.html :
    (VH-EAG : 1049F, C-121C).

(D) http://www.superconstellation.org/ :
    (N73544 : 1049F, C-121C).

(E) http://www.airliners.net/discussions/general_aviation/read.main/1738757/4/ :

(F) http://aviatechno.free.fr/constellation/ :

(G) http://www.factorypipe.com/t_brake.php :
    Power is proportional to RPM and BMEP.


4 March 2012.
