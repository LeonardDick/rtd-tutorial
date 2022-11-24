Installation
------------

To use CONAn, simply clone the public repository to your machine using using GitHub::

    $ git clone ...

The code is written in Python 3.8.10., however multiple libraries are relied on to run the code. These are listed in the requirements.txt file. To install these, run the following command::

    $ pip install -r requirements.txt

You can also manually install all packages with the following command::

    $ pip install argparse gettext os xml.dom pandas numpy math time scipy gc matplotlib.pyplot prettytable cdist

Now the code is ready to run. To run the code, simply run the following command::

    $ python3 CONAn.py
    

The code will then run and output the results to the terminal. An output.log file will be written. This file contains the same information as the terminal output, but is formatted in a way that is easier to read. The output.log file is also used to store the results of the code when running multiple simulations.