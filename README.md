# Ortiz HPC 🚀

> **Independent Studies & PoCs in High-Performance Computing (HPC)**  
> *Solving real-world problems through applied mathematics, low-level systems engineering, and hardware-level performance tuning.*

---

## 📌 About the Project

**Ortiz HPC** is an independent engineering and research initiative focused on **High-Performance Computing (HPC)**, numerical simulation, and high-throughput systems optimization.

The primary objective of this organization is to demonstrate practical technical competence in solving high-complexity scientific and industrial problems while documenting performance benchmarks, memory profiling, and parallelism execution.

### Strategic Objectives
- 🔬 **Low-Level Mastery:** Pushing hardware limits through manual memory management, cache alignment, and SIMD vectorization.
- 🧮 **Applied Mathematics:** Solving differential equations, dense/sparse linear algebra, and numerical methods.
- 🎓 **Academic Preparation:** Building a rigorous practical foundation for Master's degree research and scientific computing in HPC.
- 🌐 **Global Market Engineering:** Publicly showcasing speedup metrics and parallel efficiency across benchmarks.

---

## 🛠️ Technological Architecture (The HPC Triad)

To achieve maximum computational throughput without sacrificing analytical capability, projects adhere to a 3-layer architecture:

```text
┌────────────────────────────────────────────────────────────────────────┐
│                          1. FORTRAN (Engine)                           │
│      High-precision numerical computing, physics, and dense matrices   │
└──────────────────────────────────┬─────────────────────────────────────┘
                                   │  (C-Bindings / ISO_C_BINDING)
┌──────────────────────────────────▼─────────────────────────────────────┐
│                       2. C / C++ (Orchestration)                       │
│    Memory management, multi-core parallelism (OpenMP/MPI), C-bridge    │
└──────────────────────────────────┬─────────────────────────────────────┘
                                   │  (ctypes / CFFI / pybind11)
┌──────────────────────────────────▼─────────────────────────────────────┐
│                          3. PYTHON (Analysis)                          │
│        Data visualization, graphics plotting, and performance analysis │
└────────────────────────────────────────────────────────────────────────┘

```

| Language | Role in Ecosystem |
| --- | --- |
| **Fortran 2003/2008+** | **Numerical Core (*Engine*):** Exact execution of numerical algorithms, compute-heavy loops, and high-speed scientific calculations. |
| **C / C++ (17/20)** | **Orchestration & Low-Level:** Interoperability via *C-Bindings*, multi-core concurrency (*OpenMP*), distributed systems (*MPI*), and fine-grained memory management. |
| **Python 3** | **Visualization & Glue Code:** Invoking compiled shared libraries (`.so`/`.dll`), extracting metrics, and plotting convergence/speedup curves (*Matplotlib/Seaborn/PyVista*). |

---

## 🔄 Development Pipeline

Every PoC (Proof of Concept) or exercise within this repository strictly adheres to the following workflow:

```text
[Real-World Problem] 
       ↓
[Mathematical & Physical Modeling] 
       ↓
[Engine Implementation in Fortran] 
       ↓
[Bridge & Parallelization in C/C++] 
       ↓
[Orchestration & Plotting in Python] 
       ↓
[Profiling Report & Benchmarking]

```

---

## 📊 Rigor & Benchmarking

All projects contain a dedicated section in their local `README` featuring key engineering deliverables:

* **Mathematical Validation:** Comparing numerical outputs against analytical exact solutions.
* **Performance Metrics:** Measuring *Speedup* ($S(p) = \frac{T_1}{T_p}$) and *Parallel Efficiency* ($E(p)$).
* **Hardware Profiling:** Diagnosing bottlenecks, cache misses, and memory allocation efficiency using tools such as `perf`, `Valgrind`, and `gprof`.

---

## 👤 Author

**Ortiz David**

*Senior Software Engineer & Systems Architect*

* 🌐 **GitHub Profile:** [@ortizdavid](https://github.com/ortizdavid)
* 📝 **Dev.to:** [dev.to/ortizdavid](https://dev.to/ortizdavid)
* 💼 **LinkedIn:** [in/ortiz-david](https://www.linkedin.com/in/ortiz-david)
* ✍️ **Medium:** [@ortizaad1994](https://medium.com/@ortizaad1994)

---

*Ortiz HPC — Engineering at the Edge of Hardware.*

```
