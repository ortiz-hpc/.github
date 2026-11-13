# Mathematical Roadmap (`math.md`)

This document outlines the core applied mathematics and numerical methods required to model and discretize physical phenomena within the **Ortiz HPC** ecosystem. 

Rather than abstract or purely theoretical mathematics, this roadmap focuses exclusively on the tools needed to transform continuous differential equations into discrete, high-performance algorithms.

---

## 1. Linear Algebra & Matrix Computations
*Fundamental for solving systems of equations ($Ax = b$) in mesh-based simulations.*
* **Matrix Operations:** Matrix-vector and matrix-matrix multiplications, transposition, and factorizations (LU, Cholesky).
* **Sparse Matrices:** Storage formats optimized for memory efficiency and cache locality (Compressed Sparse Row - CSR, Compressed Sparse Column - CSC).
* **Iterative Solvers:** Linear solvers for large systems (Jacobi, Gauss-Seidel, Conjugate Gradient, BiCGStab).

## 2. Numerical Analysis & Calculus
*The bridge between continuous physical laws and discrete computer logic.*
* **Finite Difference Method (FDM):** Taylor series expansions for approximating first, second, and mixed spatial derivatives (Forward, Backward, Central differences).
* **Time Integration Schemes:** Ordinary Differential Equation (ODE) solvers for time-stepping (Euler explicit/implicit, Runge-Kutta methods like RK4).
* **Numerical Stability & Convergence:** Von Neumann stability analysis, truncation errors, and governing constraints (e.g., Courant–Friedrichs–Lewy / CFL condition).

## 3. Vector Calculus & Differential Equations
*The mathematical language of physical fields and conservation laws.*
* **Differential Operators:** Gradient, divergence, curl, and the Laplacian operator in Cartesian, cylindrical, and spherical coordinates.
* **Partial Differential Equations (PDEs):** Classification of second-order PDEs (Elliptic, Parabolic, Hyperbolic) and their physical counterparts (e.g., Laplace, Heat/Diffusion, Wave equations).
* **Boundary & Initial Conditions:** Dirichlet, Neumann, and Robin boundary conditions.
