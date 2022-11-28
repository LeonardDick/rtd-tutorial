CONAn - User Guide
===================================

.. note::

   This project is under active development.

**CONAn** is a Python program to analyze MD trajectories composed of a liquid and carbon structures.
It is the counterpart to the powerful and established program *TRAVIS* (http://www.travis-analyzer.de/).
The program is able to do the following:

* Generate carbon structures like graphene walls or carbon nanotubes (CNT).
* Set up a system from a bulk liquid and a carbon structure.
* Identify and characterize carbon structures found in the system.
* Calculate the coordination number of the liquid (inside and outside of the CNT).
* Calculate the radial density inside the CNT.
* Calculate the axial density along the CNT and bulk.

Additionally the program has a molecule identifier, which makes it possible to perform all analysis for the individual kind of molecules present in the system.

..Check out the :doc:`Installation` for more information on how to install CONAn.
  Check out the :doc:`Analysis` section for further information on the analysis.

.. toctree::
   :caption: First Steps
   :maxdepth: 2

   first_steps/Installation
   first_steps/input_output

.. toctree::
   :caption: Carbon Builder
   :maxdepth: 2

   carbon_struc/CBuilder

.. toctree::
   :caption: Analysis
   :maxdepth: 2

   analysis/Analysis
