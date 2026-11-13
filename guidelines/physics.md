# Physical Domains (`physics.md`)

This document outlines the core physical principles, governing laws, and continuum mechanics domains modeled within the **Ortiz HPC** ecosystem. 

High-performance simulations rely on translating conservation laws into discrete mathematical models that can be executed efficiently across hardware architectures.

---

## 1. Continuum Mechanics & Conservation Laws
*The foundational principles governing all macroscopic physical simulations.*
* **Conservation of Mass:** Continuity equation ensuring mass neither is created nor destroyed within a control volume.
* **Conservation of Momentum:** Newton's second law applied to continuous media (Cauchy momentum equation).
* **Conservation of Energy:** First law of thermodynamics tracking internal, kinetic, and thermal energy transfers.

## 2. Heat Transfer & Diffusion
*The baseline physical phenomenon for our initial numerical proofs of concept.*
* **Fourier's Law of Thermal Conduction:** Heat flux proportional to the negative temperature gradient ($q = -k \nabla T$).
* **The Heat Equation (Diffusion Equation):** Parabolic partial differential equation governing temperature distribution over space and time ($\frac{\partial T}{\partial t} = \alpha \nabla^2 T$).
* **Boundary & Initial Thermal States:** Modeling insulated boundaries, fixed temperatures (Dirichlet), and convective heat losses (Neumann/Robin).

## 3. Fluid Dynamics & Transport Phenomena
*Advanced domains for fluid motion and multi-phase systems.*
* **Advection-Diffusion Equation:** Combining transport of a scalar quantity by bulk fluid motion (advection) and random molecular motion (diffusion).
* **Navier-Stokes Equations:** Governing equations for viscous fluid flow (foundational for aerodynamics and weather simulation).
* **Porous Media Flow (Darcy's Law):** Fluid flow through permeable media—critical for subsurface reservoir simulation and oil/gas recovery modeling.

## 4. Stochastic & Particle Systems
*Alternative modeling paradigms for probabilistic and discrete systems.*
* **Monte Carlo Methods:** Simulating physical systems (e.g., neutron transport, molecular movement) using random sampling and statistical averaging.
