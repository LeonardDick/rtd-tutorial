CONAn - User Guide
===================================

.. note::

   This project is under active development.

**CONAn** is a Python program to generate carbon structures, set up MD simulation boxes and analyze MD trajectories composed of a liquid and carbon structures.
It shall pose as an addition to the powerful and established program *TRAVIS* (http://www.travis-analyzer.de).
The program is able to do the following:

* Generate carbon structures like graphene walls or carbon nanotubes (CNT).
* Set up a system from a bulk liquid and a carbon structure.
* Identify and characterize carbon structures found in a trajectory.
* Calculate the radial density inside a CNT.
* Calculate the accessible volume of a CNT.
* Calculate the axial density along a CNT and bulk.
* Produce xyz files of the first frame/CNT (either filled with liquid or empty) from the trajectory.

Additionally the program has a molecule identifier, which makes it possible to perform all analysis for the individual kind of molecules present in the system.

Check out the :doc:`first_steps/Installation` for more information on how to install CONAn.

.. toctree::
   :caption: First Steps
   :maxdepth: 2

   first_steps/Installation
   first_steps/input_output

.. toctree::
   :caption: Simulation Setup
   :maxdepth: 2

   simulation_setup/cbuilder
   simulation_setup/simulation_box

.. toctree::
   :caption: Picture Mode
   :maxdepth: 2

   pic_mode/picture_mode

.. toctree::
   :caption: Analysis
   :maxdepth: 2

   analysis/mol_ident
   analysis/acc_volume
   analysis/dens_prof

.. toctree::
   :caption: Other
   :maxdepth: 2

   other/versions
   other/imprint
   other/privacy_policy