# Ortiz HPC 🚀

> **Estudos Independentes & PoCs de Computação de Alta Performance (HPC)**  
> *Resolução de problemas do mundo real através de matemática aplicada, engenharia de sistemas de baixo nível e otimização física de hardware.*

---

## 📌 Sobre o Projeto

O **Ortiz HPC** é um ecossistema de engenharia e investigação independente focado em **High-Performance Computing (HPC)**, simulação numérica e otimização de sistemas computacionais de alto rendimento.

O objetivo principal desta organização é demonstrar competência técnica prática na resolução de problemas científicos e industriais de alta complexidade, documentando benchmarks de desempenho, profiling de memória e paralelismo.

### Objetivos Estratégicos
- 🔬 **Domínio de Baixo Nível:** Exploração do limite do hardware (gestão manual de memória, cache alignment, vetorização SIMD).
- 🧮 **Matemática Aplicada:** Resolução de equações diferenciais, álgebra linear densa/esparsa e métodos numéricos.
- 🎓 **Preparação Académica:** Base prática e rigorosa para nível de Mestrado e Investigação Científica em HPC.
- 🌐 **Engenharia para o Mercado Global:** Demonstração pública de métricas de aceleração (*speedup*) e eficiência paralela.

---

## 🛠️ Arquitetura Tecnológica (A Tríade de HPC)

Para garantir a máxima eficiência computacional sem abdicar da capacidade analítica, os projetos seguem uma arquitetura em 3 camadas complementares:

```text
┌────────────────────────────────────────────────────────────────────────┐
│                          1. FORTRAN (Engine)                           │
│     Cálculo numérico de alta precisão, física e matrizes densas       │
└──────────────────────────────────┬─────────────────────────────────────┘
                                   │  (C-Bindings / ISO_C_BINDING)
┌──────────────────────────────────▼─────────────────────────────────────┐
│                       2. C / C++ (Orquestração)                        │
│   Gestão de memória, paralelismo (OpenMP/MPI) e ponte de baixo nível   │
└──────────────────────────────────┬─────────────────────────────────────┘
                                   │  (ctypes / CFFI / pybind11)
┌──────────────────────────────────▼─────────────────────────────────────┐
│                          3. PYTHON (Análise)                           │
│      Geração de gráficos, visualização de dados e análise gráfica     │
└────────────────────────────────────────────────────────────────────────┘

```

| Linguagem | Responsabilidade no Ecossistema |
| --- | --- |
| **Fortran 2003/2008+** | **Núcleo Numérico (*Engine*):** Resolução exata de algoritmos numéricos, loops intensivos e cálculo científico de alta velocidade. |
| **C / C++ (17/20)** | **Orquestração & Baixo Nível:** Interoperabilidade via *C-Bindings*, concorrência multi-core (*OpenMP*), sistemas distribuídos (*MPI*) e gestão fina de memória. |
| **Python 3** | **Visualização & Glue Code:** Invocação dos binários compilados (`.so`/`.dll`), extração de métricas e geração de gráficos de convergência/speedup (*Matplotlib/Seaborn/PyVista*). |

---

## 🔄 Fluxo de Desenvolvimento

Cada PoC (Proof of Concept) ou exercício dentro deste repositório segue rigorosamente o pipeline abaixo:

```text
[Problema do Mundo Real] 
       ↓
[Modelagem Matemática & Física] 
       ↓
[Implementação da Engine em Fortran] 
       ↓
[Bridge & Paralelização em C/C++] 
       ↓
[Orquestração & Plot Gráfico em Python] 
       ↓
[Relatório de Profiling & Benchmarking]

```

---

## 📊 Rigor & Benchmarking

Todos os projetos contêm uma seção dedicada no `README` local com os seguintes entregáveis de engenharia:

* **Análise de Correção Matemática:** Comparação da solução numérica com a solução analítica exata.
* **Métricas de Performance:** Medição de *Speedup* ($S(p) = \frac{T_1}{T_p}$) e *Eficiência Paralela* ($E(p)$).
* **Profiling de Hardware:** Diagnóstico de gargalos, *cache misses* e alocação de memória usando ferramentas como `perf`, `Valgrind` e `gprof`.

---

## 👤 Autor

**Ortiz David**

*Senior Software Engineer & Systems Architect*

* 🌐 **GitHub Profile:** [@ortizdavid](https://github.com/ortizdavid)
* 📝 **Dev.to:** [dev.to/ortizdavid](https://dev.to/ortizdavid)
* 💼 **LinkedIn:** [in/ortiz-david](https://www.linkedin.com/in/ortiz-david)
* ✍️ **Medium:** [@ortizaad1994](https://medium.com/@ortizaad1994)

---

*Ortiz HPC — Engineering at the Edge of Hardware.*

```
