Density Profiles
================

For the calculation of the density profiles, the following parameters are potentially needed:

Hi

* element masses 
* van der Waals :footnote:t:'Slater1964' or atomic :cite:t:'Slater1964' (covalent) radii of the elements
* number of increments (set by the user)

.. list-table:: 
   :widths: 25 25 25 25 
   :header-rows: 1

   * - element
     - mass [u]
     - vdW radius [ang]
     - atomic radius [ang]
   * - H
     - 1.0079
     - 1.20
     - 0.25
   * - C
     - 12.0107
     - 1.70
     - 0.70
   * - N
     - 14.0067
     - 1.55
     - 0.65
   * - O
     - 15.9994
     - 1.52
     - 0.60
   * - F
     - 18.9984
     - 1.47
     - 0.50
   * - P
     - 30.9738
     - 1.80
     - 1.00
   * - S
     - 32.0650
     - 1.80
     - 1.00


Radial Denstity
-------------------
Radial densities can be computed. 
With the center line of the CNT set as origin, the space around the center is cut into increments of the users' choice, up until the tubes' wall. 
The CNT is automatically identified in the trajectory and the number of increments and therefore their volumes are set by the user. 
While scanning over the whole trajectory, every atom which is inside the CNT is identified, weighed by its element kind and sorted into the according increment given by the distance criterion.
After the scan, the obtained masses per increment are then divided by the volume of the respective increment as well as the number of time steps investigated to obtain the density. 
The results can be plotted in multiple ways, set by the user and the results are written to ``Radial_density_function.csv``. 
The analysis can be performed individually for all liquid species present.

Axial Density Profile
-------------------
Compute a density profile over the whole simulation box along the CNT axis. 
Again, as for the radial density, the CNT and all carbon structures are identified automatically in the trajectory. 
The volume of the CNT is either calculated with the accessible radius :math:`r_{acc}`, which is computed on the fly (see accessible volume) or with the radius of the CNT :math:`r_{CNT}`.
:math:`r_{CNT}` is defined as the distance between a carbon atom of the CNT and the center line of the CNT.
The number of increments and therefore their volumes are set by the user. 
As the volume of each increment in the bulk and in the pore differ, multiple regions are defined in the simulation box.
The number of increments set by the user subdivides the CNT and the bulk phases independently to assure that the calculations are done correctly.
The analysis starts by scanning the entire trajectory and sorting all atoms into a given increment, weighed by its element kind.
The obtined total increment masses are then divided by the number of frames and the respective increment volume to obtain the density.
The analysis can be performed individually for all liquid species present.
The results can be plotted if wanted and the data is written to ``Axial_density.csv``.
