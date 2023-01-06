Trajectory analysis
===================

The trajectory analysis tool is automatically called, when a trajectory is loaded. Use the '-f' flag to define which trajectory to load.
.. code-block::
    
    $ CONAn.py -f trajectory.xyz

.. note::
    The trajectory has to either xyz or pdb format. If the trajectory is in xyz format, the user is prompted to enter the simulation box dimensions, as they are needed for some analysis.
    In the case of a pdb file, the box dimensions are read directly from the file.

The analysis tool is divided into two main parts, the picture mode and the analysis mode.

Picture mode
-----------

Simulation Box Picture
^^^^^^^^^^^^^^^^^^^^^^
Save the xyz structure of the first frame of a given trajectory.

CNT Picture
^^^^^^^^^^^
Save the xyz structure of the CNT in the simulation with walls on both ends.

Filled CNT
^^^^^^^^^^
Save the xyz structure of the CNT (without the outer walls). Optionally include all atoms, which are inside the CNT.



