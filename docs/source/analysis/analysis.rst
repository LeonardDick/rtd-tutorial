Molecule identifier
===================
A molecule identifier is included in the program. It is a simple version, which deducts all bonded atoms from simple distance criteria.


Accessible Diameter
===================
The accessible diameter is obtained by scanning through the entire trajectory and identify the largest distance of an atom (including its van der Waals radius) from the center of the CNT. The accessible diameter is then twice the largest distance.


Density Profiles
================

Radial Denstity
-------------------
The radial density is obtained by scanning through the entire trajectory and identify the number of atoms (including its van der Waals radius) within a certain distance from the center of the CNT. The atoms are weighted by their mass and divided by the number of frames in the trajectory. The radial density is then plotted against the distance from the center of the CNT.

Axial Density Profile
-------------------
Compute a density profile along the CNT axis. The density profile is obtained by scanning through the entire trajectory and identify the number of atoms which belong to a certain increment defined by the user.



Coordination Number
===================
Compute the coordination number for a given molecule inside and outside the pore.
