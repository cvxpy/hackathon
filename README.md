# CVXPY Hackathon 2026

Welcome to the CVXPY Hackathon 2026! We are excited to see what you build with CVXPY.

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

Work is organized into 10 themes. Each theme has a directory under `themes/` where teams should commit their work.

### Benchmarking

Help us understand the performance profiles of the default CVXPY solvers (Clarabel, OSQP, SCS, and HiGHS). TODO link each solver
We will use your findings to improve automatic solver selection.

Reference project:
- [solver-benchmarks](https://github.com/cvxgrp/solver-benchmarks)

### Developer Tools

Improve the CVXPY developer experience by building debugging and visualization tools. 

Reference projects:
- [cvxpy-analyzer](https://github.com/cvxpy/cvxpyanalyzer)
- [cvxpy-debug](https://github.com/cvxgrp/cvxpy-debug)

### Energy

Optimization is essential to the operation of electrical grids and other power systems.
Build new packages for energy/power systems.

Reference projects:
- [cvxpower](https://github.com/cvxgrp/cvxpower)
- [emhass](https://github.com/davidusb-geek/emhass)

### Engineering Design

Many engineering design problems can be modeled as geometric programs or other types of convex programs.
Build new packages for engineering design applications.

Reference projects:
- [gpkit](https://github.com/convexengineering/gpkit)

### Finance

Convex optimization is widely used in finance for portfolio construction. Build new finance packages leveraging CVXPY.

Reference projects:
- [Cvxportfolio](https://github.com/cvxgrp/cvxportfolio)
- [PyPortfolioOpt](https://github.com/PyPortfolio/PyPortfolioOpt)

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

### Non-Convex Optimization

Build software for non-convex optimization on top of CVXPY.

Reference projects:
- [GCSOPT]
- TODO other packages from people in the workshop

### Phyical Sciences

Use CVXPY in physical sciences such as biology, chemistry, or quantum physics.

Reference projects:
- TODO quantum computing

### Other

Be creative! Any project related to optimization is welcome. It's not required to build on CVXPY.

Reference projects:
- [lpviz](https://lpviz.net/)

## Demos

Demos run from 4:15 to 5:15 (60 minutes). Demos should be 3 to 5 minutes.

## Discord

_Discord link and channel info will be posted here before the event._

## Contributing

Each team should commit their work into the appropriate `themes/<theme-name>/` directory. Create a subfolder for your project with a README describing what you built.
