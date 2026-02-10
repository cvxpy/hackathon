# CVXPY Hackathon 2026

Welcome to the CVXPY Hackathon 2026! We are excited to see what you build!

## Setup

Install CVXPY before the event: <https://www.cvxpy.org/install/>

## Schedule

| Time | Activity |
|------|----------|
| 9:00 | Welcome and introductions |
| 9:15 | Theme overview and team formation |
| 9:45 | Hacking begins |
| 12:00 | Mid-Day Check-In |
| 12:30 | Lunch break |
| 1:15 | Hacking continues |
| 4:00 | Demo prep |
| 4:15 | Demos |
| 5:15 | Wrap-up and closing |

## Themes

Work is organized into 10 themes. Each theme has a directory under `themes/` where teams should commit links to their work and any design docs produced. See `themes/benchmarks` for an example.

### Benchmarking

Help us understand the performance profiles of the default CVXPY solvers ([Clarabel](https://github.com/oxfordcontrol/Clarabel.rs), [OSQP](https://github.com/osqp/osqp), [SCS](https://github.com/cvxgrp/scs), and [HiGHS](https://github.com/ERGO-Code/HiGHS)).
We will use your findings to improve automatic solver selection.

Reference project:
- [solver-benchmarks](https://github.com/cvxpy/solver-benchmarks)

### Developer Tools

Improve the CVXPY developer experience by building debugging and visualization tools. 

Reference projects:
- [cvxpy-analyzer](https://github.com/cvxpy/cvxpyanalyzer)
- [cvxpy-debug](https://github.com/SteveDiamond/cvxpy-debug)

### Energy

Optimization is essential to the operation of electrical grids and other power systems.
Build new projects for energy/power systems.

Reference projects:
- [cvxpower](https://github.com/cvxgrp/cvxpower)
- [EECO](https://github.com/we3lab/eeco)
- [emhass](https://github.com/davidusb-geek/emhass)

### Engineering Design

Many engineering design problems can be modeled as geometric programs or other types of convex programs.
Build new projects for engineering design applications.

Reference projects:
- [gpkit](https://github.com/convexengineering/gpkit)

### Finance

Convex optimization is widely used in finance for portfolio construction. Build new finance projects leveraging CVXPY.

Reference projects:
- [Cvxportfolio](https://github.com/cvxgrp/cvxportfolio)
- [PyPortfolioOpt](https://github.com/PyPortfolio/PyPortfolioOpt)
- [Riskfolio-Lib](https://github.com/dcajasn/Riskfolio-Lib)

### Interfaces

Develop new ways to interact with CVXPY, such as visual editors, database integration, and AMPL-style APIs.

Reference projects:
- [CVXlab](https://cvxlab.readthedocs.io/en/latest/)
- [cvxpy-or](https://github.com/cvxgrp/cvxpy-or)

### Languages

The original CVX* language was [CVX](https://cvxr.com/cvx/) in MATLAB. Besides CVXPY, 
there is also [Convex.jl](https://github.com/jump-dev/Convex.jl), [CVXR](https://github.com/cvxgrp/CVXR),
and prototypes in Rust and TypeScript.
Build a simple CVX* implementation in a new language or extend one of the prototype implementations.

Reference projects:
- [CVX](https://github.com/cvxr/CVX)
- [Convex.jl](https://github.com/jump-dev/Convex.jl)
- [CVXR](https://github.com/cvxgrp/CVXR)
- [cvxjs](https://github.com/SteveDiamond/cvxjs)
- [cvxrust](https://github.com/SteveDiamond/cvxrust)

### Optimization Extensions

Build projects leveraging extensions of CVXPY for other types of optimization, 
such as GCSOPT for Graphs of Convex Sets.

Reference projects:
- [DBCP](https://github.com/nrgrp/dbcp)
- [GCSOPT](https://github.com/TobiaMarcucci/gcsopt)
- [pycvxset](https://github.com/merlresearch/pycvxset)
- [MOCVXPY](https://github.com/salomonl/mocvxpy)

### Physical Sciences

Use CVXPY in physical sciences such as biology, chemistry, or (quantum) physics.

Reference projects:
- [qiskit](https://github.com/Qiskit/qiskit)

### Other

Be creative! Any project related to optimization is welcome. It's not required to build on CVXPY.

Reference projects:
- [lpviz](https://lpviz.net/)

## Demos

Demos run from 4:15 to 5:15 (60 minutes). Demos should be 3 to 5 minutes.

## Discord

_Discord link and channel info will be posted here before the event._

## Contributing

To submit your project, create a markdown file in the appropriate `themes/<theme-name>/` directory:

1. Pick your theme directory (e.g., `themes/energy/`)
2. Create a file named after your project (e.g., `themes/energy/my-cool-project.md`)
3. Use the format shown in [`TEMPLATE.md`](TEMPLATE.md)
4. Commit and push
