Molecule identifier
===================
A molecule identifier is included in the program. 
It is a simple version, which defines all bonds between atoms from simple distance criteria. 
The cutoff distances, below which two atoms are considered bonded are depending on the element kind of the given atoms. 
All combinations of elements are listed in a library.
The program deduces all molecules from the first frame in the trajectory and therefore cannot handle bond breaking or formation in the trajectory.
First, a distance matrix is computed between all atoms in the first frame. 
Then, the cutoff matrix is computed from the cutoff distances listed in the library.
The bond matrix is computed by comparing the distance matrix with the cutoff matrix.

.. note::
    The molecule identifier is not yet able to hande PBC. 
    If the molecules have to be identified in a periodic system, the molecules have to be wrapped before.
    The library of cutoff distances is not yet complete, and cutoff distances with elements apart from C, H, N, O have yet to be implemented.


