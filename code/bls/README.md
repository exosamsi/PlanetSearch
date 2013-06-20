PyBLS
=====

Python wrapper for a multithreaded F2003 version of the EEBLS routine by Kovacs et al. (Kovacs, Zucker & Mazeh 2002, A&A, Vol. 391, 369). The original F77 routine can be found from http://www.konkoly.hu/staff/kovacs/index.html.


Install
-------
With a fairly modern gcc

	setup.py config_fc --fcompiler=gnu95 --opt="-Ofast -ffast-math" --f90flags="-cpp -fopenmp -march=native" install --user

With a bit less modern gcc

	setup.py config_fc --fcompiler=gnu95 --opt="-O3 -ffast-math" --f90flags="-cpp -fopenmp -march=native" install --user

Usage
-----

	from pybls import BLS
	...
	bls = BLS(time, flux, error)
	res = bls()
