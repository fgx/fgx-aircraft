Boeing 314A real data
=====================
Weight limits   : take-off 84000 lb (full load), landing 80000 lb (A).

Engine limits   : - maximum : 37.5 inhg 2300 rpm (1350 hp), at sea level;
                              35.8 inhg 2300 rpm (1350 hp), at 6200 ft (A).
                  - take-off (2 minutes) : 43.5 inhg 2400 rpm (1600 hp) (A).

Airspeed limits : - glide or dive 184 kt true (A).
                  - max 172 kt, cruise 160 kt (D).
                  - Vmax 201 mph [175 kt] at 6200 ft, Vcruise 184 mph [160 kt] at 11000 ft,
                    Vstall 70 mph [61 kt] (C).
                  - maximum 199 mph [173 kt], cruise 184 mph [160 kt] (B)
                  - level flight or climb 155 kt true (A).
                  - flaps extended (40 deg or less) 105 kt true (A).
                  - flaps extended (more than 40 deg) 91 kt true (A). 

Usable ceiling (A) :

Ceiling (ft)   Weight (lb)   RPM   Manifold   True IAS  Cowl flap   De-icers
                                   pressure     (kt)     opening    installed
-----------------------------------------------------------------------------
  10000         80000       2300   Full         100     5 degrees     yes
                                   throttle
   9000         84000       2300   Full         102     5 degrees     yes
                                   throttle

Ceiling : - cruise 13400 ft, maximum 19600 ft, climb 562 ft/min (E).
          - 19600 ft (D).

Range : 5200 miles [4500 NM] (B).


Operation :
- turn    : - "If you had to taxi to downwind, on the turn to downwind the wind could get under
            the upwind wing and tip the plane until the downwind wing dug into the water.
            In that condition a lot of water could flow into the wing, and once there could flow
            through the wings and into the fuselage, dousing everyone and everything.
            That never happened to me but I did hear of such cases.
            When we faced that situation we would have several of the crew walk into
            the upwind wing out to the outer nacelle, to provide balance during the turn." (F).
            - the 314 water rudder, too small for its weight, was unsatisfactory (L).
- cruise  : - "One sets up the cruise at 117 mph [102 kt], until 135 mph [117 kt] as one burns off gas.
            They were never anywhere near the advertised max cruise of 193 mph [168 kt] :
            KSFO - PHNL [2080 NM] at an average speed of 126 mph [109 kt], 16 hours depending of wind" (F).
- landing : - 70-75 mph [61-65 kt] (F).
            - the 314 had unstable skipping, which has been corrected (A-314) by moving the step aft,
            to increase the angle between forebody and afterbody, and reduce the suction (M). 



Comparison of 314 with 314A
===========================
Weight limits : take-off 82500 lb (full load) (D).
Engine at 1550 hp, slightly smaller propeller (A).
Airspeed limits : max 167 kt, cruise 158 kt (D).
Ceiling : 13400 ft (D).
Range : 3500 miles [3000 NM] (B).


314 real schedule (H)
=================
In 1939, France was GMT-0, and one must suppose that Ireland was GMT-1.

Eastbound flights are longer because of westerly winds.
Probably not direct, Lisbon - Marseille is slower.

Departure              Arrival               Lag    Westbound    Eastbound    Distance          Leg            Speed 
-------------------------------------------------------------------------------------------------------------------------
Port Washington NY     Shediac NB            1 h       4h           4h          510 NM       KLGA CYQM           128 kt
Shediac NB             Botwood NF            0 h       3h           3h          410 NM       CYQM CCP2           137 kt
Botwood NF             Foynes Ireland        3 h      11h30        16h30       1740 NM       CCP2 EINN       151/105 kt
Foynes Ireland         Southampton UK        1 h       2h30         2h30        300 NM       EINN EGHI           120 kt

Port Washington NY     Horta Azores          3 h      16h          20h         2070 NM       KLGA LPHR       129/104 kt
Horta Azores           Lisbon Portugal       2 h       7h           7h          920 NM       LPHR LPPT           131 kt
Lisbon Portugal        Marseille France      0 h       8h           8h          705 NM       LPPT LFML            88 kt

Baltimore ND           Port Washington NY    0 h       1h30         1h30        160 NM       KBWI KLGA           107 kt
Port Washington NY     Bermuda Island        1 h       5h           5h30        670 NM       KLGA TXKF       134/122 kt


314A ops
========
- parking    : - 700 RPM.
               - adjust altimeter.
               - align gyro with magnetic compass.
- taxi       : - low pitch.
               - turn with throttle on 1 outboard engine.
- take-off   : - flaps 1/3, full throttle 2400 RPM.
               - lift off between 80 kt (full load) and 60 kt (empty load). 
               - long (less than 6000 ft) because of water drag.
- climb      : - retract flaps before 105 kt.
               - reduce to 37.5 inhg (throttle), 2300 RPM.
               - 150 kt (full), 160 kt (empty).
- cruise     : - economic : 102 kt at 9000 ft (full load), 117 kt at 13400 ft (empty load).
               - maximum : 160 kt, 2300 RPM 37.5 inhg (min pitch, min mixture).
- navigation : - align gyro with magnetic compass.
               - listen in four course radio range of destination.
- descent    : - idle, max pitch.
               - increase mixture with decreasing altitude.
- approach   : flaps 1/3 below 105 kt.
- landing    : - align at 1500 ft, flaps 2/3 below 105 kt.
               - at 1000 ft, full flaps below 90 kt.
               - touch down behind the step, between 60 kt (empty load) and 75 kt (full load).
               - short because of water drag.
- stop       : 700 RPM, shutdown 2 or 4 engines.


Installation
============

Fuel load
---------
- default is maximum landing weight, 80000 lb.
- for alternate load, press "ctrl-I f" (saved on exit in aircraft-data).

Mooring
-------
- at startup, the seaplane is moved to its moorage (if any in Nasal/Boeing314-route.xml),
keeping the tower view. To disable, see "ctrl-I c".
- for alternate moorages, press "ctrl-I m".

Sounds
------
- see Sounds/Boeing314-b17-sound.xml to install B17 sounds (recommended).
- voice callouts requires Festival (festival --server in a separate shell),
  set /sim/sound/voices/enabled to true; to see the text of callouts, press "shift-F12"
  (saved on exit in aircraft-data). 


Known compatibility
-------------------
- 2.4.0 : minimal version.


Keyboard
========
- "q" : quit speed up.

Views
-----
- "ctrl-B" : "B"oat view.
- "ctrl-E" : "E"ngineer view.
- "ctrl-J" : copilot view.
- "ctrl-K" : observer view (floating).
- "ctrl-L" : boat view ("L"anding).
- "ctrl-N" : "N"avigator view (floating).
- "ctrl-O" : radi"O" view.
- "ctrl-T" : celes"T"ial view (floating).
- "shift-ctrl-T" : sex"T"ant (polaris star or southern cross).
- "shift-ctrl-V" : restore view pitch.
- "shift-ctrl-X" : restore floating view.

Virtual crew
------------
- "ctrl-W" : wind check (voice).
- "ctrl-Z" : virtual crew.
- "shift-F12"    : show crew text.
 
Unchanged behaviour
-------------------
- "x / X"  : zooms in the small fonts; reset with "ctrl-X".
- starter until slightly below 500 RPM.
  If unable to start the engine, increase the throttle beforehand, or when releasing the starter.
- "ctrl-H" : heading hold.
- "left / right" : turns the heading hold.

Same behaviour
--------------
- "S"      : swaps between Captain and Engineer 2D panels.
- "ctrl-A" : altitude hold.
- "ctrl-P" : pitch hold.
 
Improved behaviour
------------------
- "b / B"  : is the anchor, only below 15 kt.
- "up / down"  : increases / decreases pitch hold.
- "home / end" : increases / decreases pitch hold (slow).
- "page up / page down" : increases / decreases copilot speed.
- "ctrl-S" : autothrottle (virtual copilot).
- "a / A"  : speeds up BOTH speed and time; external view until X 10, internal view until X 20.
  Automatically resets to 1, when above 1000 ft/min.

Alternate behaviour
-------------------
- "ctrl-I" : menu.
- "up / down"    : move floating view in length.
- "home / end"   : move floating view in length (fast).
- "left / right" : move floating view in width.
- "page up / page down" : move floating view in height.


Mouse
=====

Autopilot
---------
- Heading hold and pitch hold are engaged separately.
- Altitude hold and pitch hold disable each other.

Four course radio range
-----------------------
Four course radio range is emulated by the NDB.
NDB only appeared after WWII with the VOR, when they both superseded the four course radio range (I).

Ground Direction Finding
------------------------
"The radio operator held the Morse key in transmit mode a minute, while the ground operator took
a bearing of the signal" (G) :
- input an airport.
- call the ground operator, by "ctrl-I d" : range is limited to 1500 miles [1300 NM] (G)(J).
- within a delay of 2 minutes, the radio returns on a paper the magnetic heading towards the airport.

Starting with the Sextant
-------------------------
Swap to sextant view, by pressing "ctrl-T" :
- activate the yellow hotspots, by pressing "ctrl-C" : the sextant should be visible,
  down at the right of the seat, in stowed position.
- take the sextant, by clicking one of the 2 cylindrical handles on its side.
- enter the sextant view, by clicking its eyepiece.
- increase field of view, by pressing "shift-X", until a notched knob is visible on the upper left.
- increase the bubble size to the maximum, by clicking this notched (bubble) knob :
  it is normal that the bubble remains out of view.
- look at the celestial pole (polaris star in northern hemisphere), by pressing "shift-ctrl-T".
- click the cylindrical (altitude) knob on the upper right, to move by step of 10 degrees,
  until the bubble enters the eyepiece : altitude-deg (on the lower left corner) should show the local latitude,
  at +/- 10 degrees.

See Instruments/BubbleSextant/README.


Virtual copilot
===============
- he aligns gyro with magnetic compass.
- he adjusts ADF to tower.
- he can hold the throttle.
- he is never the pilot in command.


Consumption
===========
Maximum speed 2300 RPM (full throttle, min pitch, min mixture), for 1 engine :
- full load, > 170 kt 86 gallons/h at 9000 ft (J = 1.05).
- empty load, > 160 kt 76 gallons/h at 13400 ft (J = 1.08).
Cruise speed 160 kt (max pitch, min mixture), for 1 engine :
- full load 2200 RPM, 74 gallons/h at 9000 ft (J = 1.02).
- empty load 2300 RPM, 70 gallons/h at 13400 ft (J = 1.05).
Economic speed, 110 kt (max pitch, min mixture), for 1 engine :
- full load 1800 RPM, 47 gallons/h at 9000 ft (J = 0.87).
- empty load 1700 RPM, 34 gallons/h at 13400 ft (J = 0.97).

As the real fuel is 1 US gal = 6 lb (A), multiply by 6.6 / 6 to compare with the real consumption.
 
All with lateral wind.
Min mixture : before engine cutoff.
Max/min pitch : before influence on RPM.

Example
-------
KSFO - PHNL, 2080 NM :
- at 0h00 zulu (afternoon), takeoff at full load (5171 gallons), heading 237 deg.
- average wind 270 deg 15 kt.
- cruise starts at 9000 ft 102 kt indicated, +1000 ft + 5 kt every 5 h,
  to reach 12000 ft 117 kt before arrival.
- ground station should be in range after 8 h.
- after 16h30, lands in the morning with 1750 gallons, or 8 h :
  130 kt average ground speed (112 kt average indicated), at 53 gallons / h.

At 160 kt indicated, the cruise will last 2080 NM / 166 kt = 12.5 h.
And the remaining fuel will be 5171 - 12.5 x 4 x 72 gallons/h = 1570 gallons or 5h30.  


JSBSim
======
- real propeller diameter (14.5 ft).
- real gear ratio 16:9.
- tilt at rest (sponsons).
- economic speed (110 kt).
- planing over step.
- rebound at landing.
- anchor.


TO DO
=====
- make 2D instruments from contemporary aircrafts.

TO DO JSBSim (seaplane)
-------------
- weathervaning at rest.
- hull stability (waterloop) with cross wind (F). 


Known problems
==============
- data are not saved on reinit.

Known problems OSG
------------------
The following artefacts are supposed to be solved by OSG :
- panels swaping too early.
- instrument transparent through layer with alpha (solved by range animation).

Known problems FDM
------------------
- above 2400 RPM at takeoff.


Secondary problems
==================
- the polaris star is barely visible; the southern cross constellation is not visible.
- the meaning of instruments is ergonomic guess and historical crosscheck.

Secondary problems FDM
----------------------
- negativ pitch at rest.
 

References
==========
(A) http://www.airweb.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/MainFrame?OpenFrameSet
    (FAA certificate, TC704 - 5 february 1941, 314A).

(B) http://www.boeing.com/history/boeing/m314.html/
    (314A)

(C) http://www.hq.nasa.gov/office/pao/History/SP-468/app-a2.htm/
    (314).

(D) http://aeroweb.brooklyn.cuny.edu/locator/manufact/boeing/bng-314.htm/
    (Differences 314 / 314A).

(E) http://www.flyingclippers.com/B314.html/

(F) http://www.southernoregonwarbirds.org/fa3.html/
    (Franck Varnum flew during WWII). 

(G) http://www.petan.net/aviation/gdf.htm
    (Marconi Adcock Direction Finder).

(H) http://bluegrassairlines.com/bgas/clip01.htm/
    (1939 PAAA schedule).

(I) http://www.navfltsm.addr.com/ndb-nav-history.htm :
    (four course radio range).

(J) http://www.panam.org/memoirs1.asp 
    (Adcock Direction Finder).

(K) http://www.pilotfriend.com/flight_training/frames2/seaplane_main_frame.htm/
    (how to fly seaplanes and amphibians).

    http://www.seaplanes.org/library/govtpubs/AC61-21A.pdf
    (seaplane operations : like (K) in pdf).

(L) http://naca.larc.nasa.gov/reports/1947/naca-tn-1387/ :
    A preliminary correlation of the behavior of water rudders on seaplanes and flying boats,
    F. W. S. Locke Jr., August 1947.

(M) http://naca.larc.nasa.gov/digidoc/report/wr/33/NACA-WR-L-333.PDF (also known as RB-3127) :
    Notes on the skipping of seaplanes,
    John B. Parkinson, September 1943.

    http://naca.larc.nasa.gov/digidoc/report/wr/04/NACA-WR-W-104.PDF :
    An analysis of the skipping characteristics of some full-size flying boats,
    F. W. S. Locke Jr., January 1946.


10 September 2011.
