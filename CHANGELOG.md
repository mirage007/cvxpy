Version 2.13 (next release)
---------------------------
* TODO get rid of NumPy 1D array warning.
* Made vstack and hstack not create new variables.
* Replaced memoize with lazyprop in constraints.

Version 2.12
------------
* Changed cvxpy to use new SCS interface.

Version 2.11
------------
* Renamed semidefinite to Semidef.
* Switched solver_specific_opts to **kwargs.
* Added vec and documentation for reshape and vec.
* Changed repr to print names in line with class names.
* Changed str for Problem.
* Made < and > map to <= and >=.
* Added warning for NumPy 1D arrays.

Version 2.10
------------
* CVXPY throws an error when a solver error is encountered.
* Presolver removes constraints with no variables.
* Conversion from non-linear constraints to linear constraints is cached. This fixes issue #122.

Version 2.9
-----------
* Fixed bug with sign multiplication.
* Added check that objective is Minimize/Maximize.
* Fixed bug with key error when solving exponential cone problem with CVXOPT.

Version 2.8
------------
* Removed a stray println.

Version 2.7
------------------------------
* CVXPY import can succeed even if SCS import fails.
* The sign of vector and matrix constant is positive (negative) if all the entries are positive (negative), instead of always being unknown.
* Can now use negative indices.
* Added *_INACCURATE return codes.

Version 2.6
-----------
* Made all lin_to_matrix functions return SciPy sparse matrix or NumPy matrix (instead of ndarray).