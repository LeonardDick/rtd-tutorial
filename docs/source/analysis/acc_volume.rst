Accessible Volume
===================
The accessible volume is calculated by scanning over the whole trajectory to identify the atom which is furthest displaced from the center line of the CNT.
The van der Waals radius is accounted for in the analysis. The accessible volume is calculated by the following equation:

.. math::

    V_{acc} = \pi*r_{acc}^2*h_{CNT}    

where r_acc is the radius of the atom which is furthest displaced from the center line of the CNT. h_CNT is the length of a given CNT.

.. note::

    The accessible volume is therefore dependent on the most displaced atom and not directly derived by the CNTs diameter.
     Results can thus slightly differ for varying simulations with the same CNT.
    


