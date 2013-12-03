Soko J-22 Orao / IAR 93
DESCRIPTION:
J-22 Orao (eng. Eagle) is a single seat twin engine
fighter-bomber aircraft. It is a result of coorporation
between Yugoslavian and Romanian flight industry. First
flight was taken in 1974, the first fight-bomber variant
was launched in 1983. J-22 (or IAR 93 in Romania) is a
low-cost aircraft and therefore appropriate for less
economical developed countries. However, it includes
some more advanced parts as well, like HUD, laser-aimed
altitude, night-vision and radion-avigation controls.
There is also a two-seat variant of this aircraft,
usually meant for piloting school.

J-22 MODEL:
I started developming the J-22 model in early 2001,
primarily for Balkans theatre, for Falcon 4.0. My
initial work started in 3D Studio MAX. However,
Falcon slowly started to die-out in those days and
I wanted something more opened and free to work for.
Then I heard about the FlightGear project, so I said
why not try to export my model to this game as well.
So, my work continued in Blender, under Linux. I
completely remade and mostly improve the mesh.
(Falcon's graphic engine was pretty weak in comparison
to FlightGear) In August 2003, I finally managed to
get my Eagle flying! The major problems now left are
some advanced model animation, 3d cockpit and maybe
some electrical/weapon/radar systems (I don't have
much info on this aircraft about this).

LICENSE:
J-22 model and all its contents are licensed under
terms of GNU/General Public License.

FlightGear J-22 MODEL STRUCTURE:
J-22 model itself consists of textures (all in .rgb format)
and j22.ac mesh model. The animation FlightGear wrapper
is $FG_ROOT/Aircraft/j22/Models/j22.xml file. It includes
all the animations and other main descriptive stuff for FG.
I named non-moving objects with lower-case and moving
objects with upper-case. I didn't use any blanks, but
seperated two words by writing the second one with upper-case.
I indexed objects by simply appending 01, 02, 03 or 001, 002,
003 numbers after object's name, without any dot between
object name and index. I named directions and positions (right
flaps, left flaps) by objectname.position (i.e. flaps.right
for the right flaps and flaps.left for the left ones).
The flight model wrapper file is j22-yasim.xml in
$FG_ROOT/Aircraft-yasim folder. The main J-22 FG set is
$FG_ROOT/Aircraft/j22-set.xml.


If you want the source .blend model or any other information,
I'll be glad to help. Enjoy flying my model!
- Matevz Jekovec
 (matevz.jekovec@guest.arnes.si)
