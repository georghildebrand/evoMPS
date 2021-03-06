===================
 Installing evoMPS
===================

Obtaining the Latest Software
-----------------------------

The latest version of evoMPS can be downloaded from 
GitHub <http://github.com/amilsted/evoMPS>.


Prerequisites
-------------

On Windows, an easy way to obtain everything required is to download and
install a numerics-oriented Python distribution such as

* pythonxy <http://www.pythonxy.com> (open source and a free download of 32-bit binaries)
* enthought python distribution <http://www.enthought.com/products/epd.php> (free for academic use, with optimized linear algerba, 64-bit available)

The full installation of either of these includes everything you need.
Otherwise, the following are required:

* Python 2 <http://www.python.org> (tested on Python 2.7)
* Numpy <http://numpy.scipy.org> (tested on 1.6.1)
* Scipy <http://www.scipy.org> (version 0.7.0 or newer - tested on 0.10)

Numpy should be compiled with a LAPACK library, preferably
an optimized one such as ATLAS <http://math-atlas.sourceforge.net/>. 
Scipy requires a LAPACK library to be present.

If present, Cython <http://www.cython.org/> will also be used to perform
some (currently minor) optimizations.

To run the included examples, the following is also required:

* matplotlib <http://matplotlib.sourceforge.net/> (tested on 1.1.0)


Building and Installation
-------------------------

To install the evoMPS package, go to the source directory and run::

    python setup.py install

Alternatively, to install for the current user only, run::

    python setup.py install --user 

Installation is not strictly necessary, as scripts using evoMPS can
also be run from the base source directory.

Getting Started
---------------

Examples have been provided in the examples/ subdirectory. After installing
evoMPS as described above, they can be run using e.g.::

    python transverse_ising.py

To run an example without installing, copy it to the base source directory first.
