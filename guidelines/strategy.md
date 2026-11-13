# Execution Pipeline (`strategy.md`)

This document defines the mandatory engineering workflow for every Proof of Concept (PoC) and simulation project within the **Ortiz HPC** ecosystem. 

To ensure absolute technical rigor and prevent premature coding, every project must follow this sequential pipeline:

```text
[ 1. Real-World Physical / Computational Problem ]
                       ↓
[ 2. Governing Equations & Mathematical Modeling ]
                       ↓
[ 3. Numerical Discretization & Stability Analysis ]
                       ↓
[ 4. Core Numerical Engine Implementation (Fortran) ]
                       ↓
[ 5. Low-Level Integration & Parallelization (C/C++) ]
                       ↓
[ 6. Orchestration, Validation & Visualization (Python) ]
                       ↓
[ 7. Hardware Profiling & Benchmarking (Speedup / Cache) ]

```

---

## Pipeline Stages

### 1. Real-World Problem Definition

* Define the physical domain, boundary conditions, and engineering objectives (e.g., thermal diffusion, fluid flow in porous media).

### 2. Governing Equations

* Identify the exact differential or algebraic equations governing the phenomenon (e.g., Fourier's Law, Navier-Stokes, Advection-Diffusion).

### 3. Numerical Discretization & Stability

* Choose the appropriate numerical method (e.g., Finite Difference Method - FDM, Finite Element Method - FEM).
* Derive algebraic approximations and calculate stability constraints (e.g., Courant–Friedrichs–Lewy / CFL condition).

### 4. Engine Implementation (Fortran)

* Write the high-performance numerical kernel using Modern Fortran (`iso_fortran_env`, explicit typing, contiguous memory layouts).

### 5. Bridge & Parallelization (C / C++)

* Expose routines via ISO C bindings.
* Implement multi-core parallelism (`OpenMP`) or distributed computing (`MPI`) where applicable.

### 6. Analysis & Visualization (Python)

* Invoke compiled shared libraries (`.so`/`.dll`), extract performance metrics, and plot convergence profiles or spatial distributions.

### 7. Profiling & Optimization

* Run hardware profiling tools (`perf`, `valgrind`, `gprof`) to analyze cache behavior, memory alignment, and execution bottlenecks.

```
