General Information
===================

The trajectory analysis tool is automatically called, when a trajectory is loaded. Use the '-f' flag to define which trajectory to load.
.. code-block::
    
    $ python3 CONAn.py -f trajectory.xyz

.. note::
    The trajectory has to either xyz or pdb format. If the trajectory is in xyz format, the user is prompted to enter the simulation box dimensions, as they are needed for some analysis.
    In the case of a pdb file, the box dimensions are read directly from the file.

As a first step, the program analyzes the trajectory regarding its size, number of frames, number of atoms in the system and more.
The user is then prompted to select a frame which is to be used to identify all rigid carbon structures in the system.
The trajectory analysis tool is divided into two main parts, the picture mode and the analysis mode, which includes all the analysis functions performed on the trajectory.
All modi will be discussed in further detail in the following sections.

For the analysis options implemented, the following parameters are potentially needed:

* element masses
* van der Waals [1]_ or covalent [2]_ radii of the elements
* number of increments (set by the user)

.. list-table:: 
   :widths: 25 25 25 25 
   :header-rows: 1

   * - element
     - mass [amu]
     - vdW radius [ang]
     - covalent radius [ang]
   * - H
     - 1.008
     - 1.20
     - 0.25
   * - C
     - 12.011
     - 1.70
     - 0.70
   * - N
     - 14.007
     - 1.55
     - 0.65
   * - O
     - 15.999
     - 1.52
     - 0.60
   * - F
     - 18.998
     - 1.47
     - 0.50
   * - P
     - 30.974
     - 1.80
     - 1.00
   * - S
     - 32.065
     - 1.80
     - 1.00


.. note::

        The user is prompted to choose between the van der Waals radii and covalent radii of the elements.
        For all analysis functions, the listed atomic masses were used.



.. [1] J.C. Slater, Atomic radii in crystals, J. Chem. Phys. 41 (10) (1964) 3199-3204.
       DOI: https://doi.org/10.1063/1.1725697
.. [2] A. Bondi, van der Waals Volumes and Radii, J. Phys. Chem. 68 (3) (1964) 441-451.
       DOI: https://doi.org/10.1021/j100785a001
