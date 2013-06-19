PyBLS
=====

Python wrapper for a multithreaded version of the Kovac's fortran BLS routine. 

Install
-------

	setup.py config_fc --fcompiler=gnu95 --opt="-Ofast -ffast-math" --f90flags="-cpp -fopenmp -march=native" install --user
