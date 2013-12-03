SU-37 (YASim) readme.

This is not intended to be an accurate representation of an SU-37 but
of an SU-37 'type' aircraft.  The SU-37 designation applies as much
to the weapons management and control systems as it does to the
airframe design and control systems.

This FG aircraft should be regarded as experimental.  While it is
based upon the SU-37, and tries to include _some_ of it's control
system features, it should be remembered that is very much an
experimental development test-bed.

AP/FCS Instrument
=================
The AP/FCS instrument, available on the mini panel allows most of
the autopilot/flight control systems functions to be engaged or
switched off.  It doesn't make any provision for changing settings
so these must be done via the existing dialogues or through the
property browser.

Basically, if something on this instrument is coloured green or red
it can be 'clicked' by the mouse to toggle the state - green = off
and red = engaged.

The legends for the controls (not all of which currently work) is below

Autopilot
  Altitude
    AH  Altitude hold
    TF  Terrainf follow
    PH  Pitch hold
    AO  AoA hold
    VC  Climb-rate hold
    GS  Glide-slope hold
    MC  Mach-climb

  Heading
    WL  Wing-leveler
    TH  True heading-hold
    DG  DG heading hold
    NV  Nav1 hold

FCS
  SMode
      DR                    Direct - stick controls pitch and roll deflection
                            elevons and flaperons directly.
      PT                    Pitch - stick controls pitch angle and roll settings.
      VC                    VFPS - stick controls climb and roll setings.

    Auto take-off/landing
      TO                    Auto take-off
      LD                    Auto landing
  AF                        Auto flaps
  AS                        Auto slats
  SB                        Auto speedbrake
  AR                        Auto reheat





YASim control input bindings
============================
Object      Control     Axis

wing        FLAP0       /autopilot/FCS/controls/flaperon-flap-norm
wing        FLAP0       /autopilot/FCS/controls/flaperon-roll-norm
wing        SLAT        /autopilot/FCS/controls/slats-norm

hstab       FLAP0       /controls/flight/elevator-trim
hstab       FLAP0       /autopilot/FCS/controls/elevon-pitch-norm
hstab       FLAP0       /autopilot/FCS/controls/elevon-roll-norm

vstab (L)   FLAP0       /autopilot/FCS/controls/rudder-norm
vstab (R)   FLAP0       /autopilot/FCS/controls/rudder-norm

mstab       SPOILER     /autopilot/FCS/controls/spoiler-norm

jet (L)     THROTTLE    /autopilot/FCS/controls/engines/engine[0]/throttle-norm
jet (L)     REHEAT      /autopilot/FCS/controls/engines/engine[0]/reheat-norm
jet (L)     VECTOR      /autopilot/FCS/controls/engines/engine[0]/vector-norm

jet (R)     THROTTLE    /autopilot/FCS/controls/engines/engine[0]/throttle-norm
jet (R)     REHEAT      /autopilot/FCS/controls/engines/engine[0]/reheat-norm
jet (R)     VECTOR      /autopilot/FCS/controls/engines/engine[0]/vector-norm

YASim control output bindings
=============================
Object      Control     Axis

wing        FLAP0       /surface-positions/left-flaperon-pos-norm
wing        FLAP0       /surface-positions/right-flaperon-pos-norm
wing        FLAP0       /surface-positions/flaperon-pos-norm
wing        SLAT        /surface-positions/left-slat-pos-norm
wing        SLAT        /surface-positions/right-slat-pos-norm
wing        SLAT        /surface-positions/slat-pos-norm

hstab       FLAP0       /surface-positions/left-elevon-pos-norm
hstab       FLAP0       /surface-positions/right-elevon-pos-norm
hstab       FLAP0       /surface-positions/elevon-pos-norm

vstab (L)   FLAP0       /surface-positions/left-rudder-pos-norm
vstab (R)   FLAP0       /surface-positions/right-rudder-pos-norm

mstab       FLAP0       /surface-positions/spoiler-pos-norm

jet (L)     THROTTLE    /engines/engine[0]/throttle-norm
jet (L)     REHEAT      /engines/engine[0]/reheat-norm
jet (L)     VECTOR      /engines/engine[0]/vector-norm

jet (R)     THROTTLE    /engines/engine[0]/throttle-norm
jet (R)     REHEAT      /engines/engine[0]/reheat-norm
jet (R)     VECTOR      /engines/engine[0]/vector-norm


FCS Listeners
=============
axis                            Listener

/autopilot/FCS/locks/engines    SU37FCSLOCKS.engines_lock_monitor
/autopilot/FCS/locks/fcs        SU37FCSLOCKS.fcs_lock_monitor
/autopilot/FCS/locks/flaps      SU37FCSLOCKS.fcs_flaps_monitor
/autopilot/FCS/locks/pitch      SU37FCSLOCKS.pitch_lock_monitor
/autopilot/FCS/locks/roll       SU37FCSLOCKS.roll_lock_monitor
/autopilot/FCS/locks/speed      SU37FCSLOCKS.speed_lock_monitor
/autopilot/locks/altitude       SU37APLOCKS.altitude_lock_monitor
/autopilot/locks/heading        SU37APLOCKS.heading_lock_monitor
/autopilot/locks/speed          SU37APLOCKS.speed_lock_monitor
/controls/flight/aileron        SU37FCSFLIGHT.aileron_monitor
/controls/flight/elevator       SU37FCSFLIGHT.elevator_monitor
/controls/flight/flaps          SU37FCSFLIGHT.flaps_monitor
/controls/flight/slats          SU37FCSFLIGHT.slats_monitor
/controls/flight/spoiler        SU37FCSFLIGHT.spoiler_monitor
/orientation/alpha-deg          SU37ORIENTATION.aoa_monitor
/position/altitude-ft           SU37POSITION.altitude_monitor
/position/altitude-agl-ft       SU37POSITION.agl_monitor
/velocities/airspeed-kt         SU37VELOCITIES.kias_monitor
/velocities/mach                SU37VELOCITIES.mach_monitor





Lee Elliott.     2006/10/11
