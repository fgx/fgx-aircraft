LOCKHEED F-104C STARFIGHTER, v. 1.2, 10 Feb 2010, released under Creative Commons license CC-BY-NC-SA

CHANGES FROM V. 1.1:

1.  Corrects faulty airspeed indication.
2.  VVI now uses FDM data for a more instantaneous indication.


ACKNOWLEDGEMENTS:

1.  The FDM is my work, derived from the current Aeromatic program.

2.  The airframe 3D is based on Emmanual Baranger's NF-104A (released under GNU General Public License v. 2).

3.  Polished metal and tire-smoke effects are based on A.J. MacLeod's BAC Lightning F1.A (released under GNU General Public License v. 2).

3.  Pilot and afterburner nozzle/flame 3Ds are based on Gerard Robin's SR-71 (released under GNU General Public License v. 2).

4.  Gun effects and submodels/systems are based on David Culp's work (released under Creative Commons license CC-BY-NC-SA), with the exception of the M61.wav, which was freeware from SoundBible.com that I edited.
NOTE: This has been removed from the CVS version. For the full version see:
      http://home.comcast.net/~davidculp2/hangar/hangar.html

5.  If you recognize your work in this model and I haven't acknowledged it, it's because of my oversight rather than intent.  Please e-mail me at k_esbenshade@hotmail.com and point out my error.  I'll attribute you here.

INSTRUMENTATION NOTES (TOGGLE CONTROL-C FOR PANEL LOCATIONS):

-- Attitude Indicator: Includes horizon adjust click panels on each side of the knob.  Click the knob itself to reset to zero.

-- Auto ILS (control-i): For the lazy among us, flies localizer, glide slope, and airspeed.  You need to be in the reasonable vicinity of all three before you activate the function.

-- Autopilot: Retuned version of the FlightGear generic autopilot for better responsiveness to fighter aircraft.

-- Altimeter:

	Local Weather Fetch Enabled:  Using a Nasal aplet, automatically sets local barometric pressure below 18,000 feet and 29.92, the standard datum plane for pressure altitude in the United States, above 18,000 feet (change-over altitude is different elsewhere).  Indicated altitude is local below 18,000 feet and pressure altitude above 18,000 feet. The autopilot uses indicated altitude for computations.

	Local Weather Fetch Disabled:  Pilot sets manually, and autopilot uses indicated altitude for computations.

-- Approach Speed Indicator:  Using a Nasal aplet, a small triangle on the outside edge of the airspeed face automatically indicates approach speed (170 KIAS plus 5 KIAS for every 1000 pounds of fuel over 1000 pounds).  Just control your airspeed to keep the needle on the approach speed indicator.

-- External stores (tip tank) jettison and arrestor hook release buttons are clickable in the cockpit.

-- Light Panel: On the right console at the 3 o'clock position.

-- Radar: Currently displays only the tanker and a 20-mile range.

-- Radio Direction Magnetic Indicator (RDMI): Displays both TACAN (wide needle) and VOR (narrow needle).

-- Refueling: Probe capable with KA-6D (refueling_demo_2 in FlightGear).
