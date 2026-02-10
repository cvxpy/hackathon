# Benchmarking Theme

## Why benchmarking matters

CVXPY ships with several default solvers —
[Clarabel](https://github.com/oxfordcontrol/Clarabel.rs),
[OSQP](https://github.com/osqp/osqp),
[SCS](https://github.com/cvxgrp/scs), and
[HiGHS](https://github.com/ERGO-Code/HiGHS) — but today the automatic solver
selection logic is rudimentary. It picks a solver based on problem type (LP, QP,
SOCP, SDP, MIP) without considering problem structure, size, or sparsity.

By collecting benchmark data across a wide range of problems **and** machines we
can build a much better solver selector that routes each problem to the solver
most likely to solve it quickly and reliably. Your contributions directly feed
into this effort.

## Reference project

All benchmark work lives in the
[solver-benchmarks](https://github.com/cvxpy/solver-benchmarks) repository.
That repo contains:

- A problem registry with `@register_problem` decorator
- A runner that times compilation, setup, and solve phases
- JSONL result storage for easy cross-machine comparison
- Analysis scripts for comparing solvers

See the solver-benchmarks
[CONTRIBUTING.md](https://github.com/cvxpy/solver-benchmarks/blob/main/CONTRIBUTING.md)
for full setup and contribution instructions.

## What problems to add

If you're solving a CVXPY problem for your work or research, we probably want a
benchmark version of it. The best benchmarks are representative of what real
users are actually solving. We want coverage across all problem types (LP, QP,
SOCP, SDP, MIP) and a range of sizes.

Good benchmark problems are:

- **Reproducible** — use `np.random.default_rng(seed)`, never global random
  state.
- **Self-contained** — the `@register_problem` factory builds its own data from
  the seed.
- **Non-trivial** — should take at least ~0.01 s to solve so timing noise
  doesn't dominate.

## What machines to run benchmarks on

**If you're solving CVXPY problems on a computer, we want benchmark data for
that computer!** Solver performance varies significantly across hardware, and the
more diverse our data the better our solver selection heuristics will be.

Some examples of machines we'd love data from:

- **Laptops** — Apple Silicon (M1/M2/M3/M4), Intel x86, AMD x86
- **Cloud instances** — AWS (c5, m5, etc.), GCP, Azure
- **Workstations** — multi-core desktop CPUs
- **Different OSes** — macOS, Linux (Ubuntu, Fedora, etc.), Windows/WSL

The runner records CPU info, OS, and Python/solver versions automatically, so
just run the benchmarks on whatever machine you have and submit the results.

## TODO

Problems:

- [ ] Add more LP, QP, SOCP, SDP, and MIP problems drawn from real use cases
- [ ] Add small, medium, and large variants of each problem
- [ ] Add stress tests (very sparse, very dense, ill-conditioned, near-infeasible)

Data collection:

- [ ] Run benchmarks on diverse hardware (Apple Silicon, Intel, AMD, cloud)
- [ ] Run benchmarks on diverse OSes (macOS, Linux, Windows/WSL)

Analysis:

- [ ] Compare solver reliability and speed across problem types
- [ ] Identify problems where solver choice matters most
- [ ] Draft recommendations for improved automatic solver selection
