# DNSimb solver
DNS code that employs a not-yet-published immersed boundary method.
At this stage, the boundary conditions are hard coded and refer to the geometry of a nasal cavity. The original aim of this code is in fact to provide medical personnel with a quick and easy-to-use code to perform patient-specific-simulations on the flow within the nasal cavity.
<p align="center">
<img src="https://user-images.githubusercontent.com/58366962/218584599-6bb14f12-03d1-41a2-bbd1-0d18df4dfdf4.png" align="center" width="500" />
</p>

Hence, the decision to use an immersed boundary method that totally removes the need for a mesh and allows for very fast code that uses little memory.

## Numerical description
- Staggered-grid
- Second order accurate finite differences
- Third order accurate, three-stage Runge–Kutta method

## Comparison with OpenFOAM
With the same number of cells, 40-45x speed improvement per iteration and 77% memory usage reduction.

Written in CPL (https://cplcode.net/, https://arxiv.org/abs/2012.12143).
