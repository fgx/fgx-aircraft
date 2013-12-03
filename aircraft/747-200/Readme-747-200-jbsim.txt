747-200  real data
==================
Weight limit (A) :
    maximum (takeoff)     : 833000 lb.
    landing (recommended) : 630000 lb.

VMO/MMO : 375/0.92 (A).
VNE/MNE : 445/0.95 (B).

Ceiling : 45100 ft (C).


747-200 ops
===========
- takeoff : - rotation 180 kt (full load), 170 kt (landing load), flaps 20 (D1).
            - trim before engaging autopilot.
- climb   : - flaps retraction scheduled with autothrottle (D2).
            - 1000 ft/min, 220 kt until 5000 ft (G).
            - 300 kt above 10000 ft (G).
            - 1500 ft/min until FL150 (G).
            - 1200 ft/min until FL240 (G).
            - 1000 ft/min, 0.82 mach until cruise (G).
- cruise  : - 0.84 mach.
- descent : - start at 250 NM.
            - 1000 ft/min, 0.84 mach until FL240 (G).
            - 1000 ft/min, decelerate to 290 kt until FL100 (G).
            - 1000 ft/min, 250 kt until approach (G).
- approach: - 160 kt (landing load), 150 kt (empty tank), flaps 20.
- final   : - 160 kt (landing load), 150 kt (empty tank), flaps 30.
            - arm spoilers.
- landing : - 154 kt (landing load), 140 kt (empty tank) (D1).
            - touch down below 400 ft/min.


Installation
============
Fuel load
---------
- default is maximum landing weight, 630000 lb.
- for alternate load, press "ctrl-I f" (saved on exit in aircraft-data).

Known compatibility
-------------------
- 2.12 : minimal version.



Keyboard
========
- "q"   : quit speed up.

Views
-----
- "ctrl-E"   : "E"ngineer view.
- "ctrl-J"   : "C"opilot view.
- "ctrl-K"   : "O"bserver view (floating).
- "shift-ctrl-V" : restore view pitch.
- "shift-ctrl-X" : restore floating view.

Same behaviour
--------------
- "F12" : radio frequencies.
- "S"   : swaps between Captain and Center 2D panels.
- "left / right" : autopilot heading.
 
Improved behaviour
------------------
- "a / A"  : speeds up BOTH speed and time. Until X 15.
             Automatically resets to 1, when above 2000 ft/min.
- "up / down"  : increases / decreases altitude hold, vertical speed hold.
- "home / end" : increases / decreases (slow) altitude hold, vertical speed hold.
- "page up / page down" : increases / decreases speed hold, Mach hold.

Alternate behaviour
-------------------
- "ctrl-I" : menu.
- "ctrl-T" : toggle altitude hold.
- "left / right" : move floating view in width.
- "up / down"  : move floating view in length.
- "home / end" : move floating view in length (fast).
- "page up / page down" : move floating view in height.

Disabled
--------
- "ctrl-P".
- "ctrl-W".


Mouse
=====

ADF
---
To update the frequency of ADF 2 :
- press "swap" on the overhead.
- press "ctrl-R" to call the radio menu. 

Autopilot
---------
- avoid default autopilot setting (F10 key), use 2D panel or 3D cockpit.


Consumption
===========
Cruise Mach 0.84 for 1 engine :
- full load, 900 gallons/h at 30000 ft.
- empty fuel, 1050 gallons/h at 38000 ft.

All with lateral wind.

Example
-------
KMSP - RJAA (E), 5300 NM :
- load --flight-plan from Doc.
- at 12h45 zulu (morning), takeoff at full load (55212 US gal).
- warm, with light adverse alofts.
- cruise starts at 30000 ft, +2000 ft every 2h30, until 38000 ft.
- after 11h45, lands in the morning with 8200 gallons (1000 gallons/h); or 2h / 920 NM.

Typical city pair (F) KJFK - RJAA (6000 NM) is not possible at full load (A).


JSBSim
======
- geometry is real data.
- center of gravity inside corridor.
- extended range 7500 NM (6200 NM at full load), without wind (A).
- 747 coefficients.


TO DO
=====
- 3D instruments.
- systems.


Known problems
==============
- data are not saved on reinit.
- use turn at maximum angle, only to stop taxi.
- from Mach 0.82, Mach drag delays altitude modes, when velocity increases.
- approach steady below the glide slope, otherwise descent overspeed triggers inertia roll. 

Known problems FDM
------------------
- descent rate too slow (G) ?

Known problems autopilot
------------------------
- toggle INS mode, only AFTER activation of route, or use "ctrl-I a".
- NAV hold mode is sensitive to the turbulence of the ground layer.
- heading hold is a little slow to converge.
- beyond 15 NM, nav hold makes wide rolls.
- yoke rolls with nav hold.

Known problems 2.4.0 autopilot
------------------------------
- heading modes may start to bank into the opposite direction.

Known problems autoland
-----------------------
- nav must be accurate until 0 ft AGL : KSFO 28R, RJAA 34L are correct;
  but EGLL 27R, KJFK 22L are wrong : to land at these airports,
  set /controls/autoflight/real-nav to false, by "ctrl-I a".
- glide slope must be accurate until 250 ft AGL : real should be 100 ft,
  but nose tends to dive to catch the slope (simplistic autopilot or wrong glide slope ?).

Known problems keyboard
-----------------------
- because of ctrl-I overriding, TAB altimeter menu is not available with GLUT.

Known problems OSG
------------------
The following artefacts are supposed to be solved by OSG :
- panels swaping too early.
- instrument transparent through layer with alpha (observer view).


References
==========
(A) http://www.boeing.com/ :
    (747 airplane characteristics, D6-58236 - May 1984).

(B) http://www.bh.com/companions/034074152X/appendices/data-a/table-3/table.htm :

(C) http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/MainFrame?OpenFrameSet :
    (FAA certificate, a20we - 23 December 1970, 747-200B).

(D1) http://www.airliners.net/discussions/tech_ops/read.main/52218/6/#ID52218 :
    V2 190 kt (max takeoff load), climbs with no flaps at V2 + 100 kt, VREF 154 kt (max landing load).

(D2) http://www.airliners.net/discussions/tech_ops/read.main/72686/6/#ID72686 :
    retract V2 + 80, for maneuver V2 + 100; extend Vref + 80.

(E) http://www.airlineroutemaps.com/USA/Northwest_Airlines.shtml :
    KDTW - RJAA is 5800 NM.

(F) http://www.boeing.com/ :
    747 Classics.

(G) http://elearning.ians.lu/aircraftperformance/ :

(H) http://www.flight-manuals-on-cd.com/747.html :



29 September 2013.
