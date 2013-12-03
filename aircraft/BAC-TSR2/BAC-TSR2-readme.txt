TSR2 yasim readme.

This is not an authentic representation of a TSR2 but it's based
on the right numbers, where I could find them.

Flying notes
------------
The real aircraft used settings of 35 deg for take-off and 50
deg for landing.  Assuming that the 50 deg setting corresponds
to full flap deflection (1.0) the 35 deg setting equates to 0.64

It's not necessary to use reheat for take-off, and infact, early
problems with the Olympus engines while in development precluded
it's use - reheat was not used until the 14th test flight.

It's possible to use the Autopilot to take-off, by selecting the
'TO' region of the AP Mode instrument with the mouse on the vfr
or mini panal.  This will hold the a/c at the correct pitch for
take-off during the take-off run but as this is a pitch-hold
based control, it will bring the nose up as soon as it can, which
is rather too early, if engaged as soon as the take-off run is
started.

The take-off controller is also unstable at higher speeds
(> 250 ias) so this control should be disengaged above this speed.
This can be done by either selecting another AP mode
i.e. Altitude-Hold (AH) or Terrain-Follow (TF), or by disengaging
the AP entirely (click the 'AP Mode:' region of the instrument).

Note:  The Autopilot is in an early state of development, and
while it's mostly usable, there are still some problems with it.

The approach AoA should be kept to around 9 deg and as the a/c
speed drops and the AoA increases, more flaps should be applied
until they are fully deployed.  Depending on the weight of the
a/c - that is, how much fuel is remaining - the approach speed
should be between 145 and 120 kias.

After switching to manual control during the final stages of
the approach, you should gently start lifting the nose at
between 100 - 50 ft agl to reduce the rate of descent and avoid
bouncing back into the air on touch-down.  The engine power should
be cut just before touching the ground and once you're down it'll
be necessary to depress the elevator a little to get the nose
wheel down on the ground.  The speed-brakes can then be used to
slow the a/c down and reduce the roll-out distance.  The real a/c
routinely used a braking parachute during it's test flights.

The TSR-2 was designed to operate at high sub-sonic speeds and
at altitudes as low as 90m using a Terrain Following (TF) system
incorporating a look-ahead TF radar.  This meant that the a/c was
aware of the ground elevation up to two miles ahead of it and not
just the agl below the a/c, which is all we currently have in FG.

As a consequence, the TF behaviour in FG isn't realistic as the
look-ahead capability in the real TF system removed the need for
sudden climbs over high ground elevations - the high elevation
would have been 'seen' ahead of the a/c and the TF system would
start the necessary climb so that the a/c would pass over the
obstacle in a nearly level attitude, making it possible to start
the following descent immediately the obstacle had been cleared.
This avoided any need to climb higher than was absolutely
necessary, it allowed the a/c to get back down again as quickly
as possible and made the a/c much more comfortable for the crew,
increasing it's endurance in this area.  The TSR-2 is quite a big
aircraft and has a high wing loading, also designed to increase
crew comfort, and therefore endurance, at low-level by reducing
the effect of wind buffet but this means that it's not a
particularly manueverable a/c - it's certainly not a fighter.

Because of the YASim solver does not currently model
trans-sonic and super-sonic aerodynamic effects, more attention
has been paid to the high-subsonic realm, although it has
sufficient power to achieve super-sonic flight without reheat, as
was the real a/c.

Lee Elliott.
