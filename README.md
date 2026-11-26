### Scott Cochran

I work on AI Safety using formal methods, policy as code, and assisted development. 

I use AI to make AI safer and easier to work with.

#### Agentic AI, safe by design

- **[TOPAK](https://github.com/scottcochran/TOPAK)** is an architecture pattern for "Safe by Design" agentic AI collaboration. It treats every agent as Byzantine and keeps models out of the trusted computing base using [TLA+, OPA, Cedar, and Paxos](https://grippinghand.dev/topak).

#### TLA+
- **[tla-kit](https://github.com/scottcochran/tla-kit)**: the TLA+ tools (TLC, TLAPS and its solvers) in one
container image pinned by digest, so the checker and the prover are the same build on a laptop and in CI. It
includes an MCP server, so an agent such as Claude Code can check a spec, read a counterexample and repair a
proof.

#### Proof posters

These are click-navigable posters of Lean and TLA proofs. They adapt to light and dark themes, are pinned to source, and reproducibly generated. Each one is released by version tag with checksums.

- **[riemann-diagrams](https://scottcochran.github.io/riemann-diagrams/)**: twenty posters of the theorem
dependency graph of Alpöge's Lean proof of the Riemann Hypothesis. They show the proof [chapter by chapter](https://scottcochran.github.io/riemann-diagrams/diagrams/R2-chapters-2026.11.23.svg), [single
chains](https://scottcochran.github.io/riemann-diagrams/diagrams/T2-trace-landau-2026.11.23.svg) of [reductions](https://scottcochran.github.io/riemann-diagrams/diagrams/T1-trace-deepest-2026.11.23.svg), its [definitions](https://scottcochran.github.io/riemann-diagrams/diagrams/R1-main-theorems-2026.11.23.svg), its [literature](https://scottcochran.github.io/riemann-diagrams/diagrams/F4-literature-2026.11.23.svg), and [what's "new"](https://scottcochran.github.io/riemann-diagrams/diagrams/F2-new-2026.11.23.svg). 

- **[riemann-masullo-diagrams](https://scottcochran.github.io/riemann-masullo-diagrams/)**: posters of the
  riemann-masullo Lean formalisation of A. M. Masullo's *The Music of the Primes*. They show what in it rests on
  the [steps no one knows how to repair](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M2-no-repair-2026.11.25.svg): the [cone of each open step](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M2-no-repair-2026.11.25.svg), the [paper by depth below its target theorems](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M3-depth-2026.11.25.svg),
  and the [printed claims the Lean refutes](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M5-refuted-2026.11.25.svg).

- **[anthropic-vp-vnp](https://scottcochran.github.io/anthropic-vp-vnp/)**: posters of *VP ≠ VNP over every field*
  and its Lean 4 formalization in [anthropics/formal-math](https://github.com/anthropics/formal-math/tree/main/vp-vnp).
  They show the proof [section by section](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/R2-sections-2026.11.25.svg),
  [the route to the main theorems](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/R3-route-2026.11.25.svg),
  [the paper against the Lean](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/F1-paper-lean-2026.11.25.svg),
  and the paper's own [Figure 1, checked](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/F4-figure-1-2026.11.25.svg)
  arrow by arrow against the Lean.

- [proof-posters](https://github.com/scottcochran/riemann-diagrams/tree/main/plugins/proof-posters) is my Claude Code plugin which was used to build the posters.

- **[gov-tla](https://scottcochran.github.io/gov-tla/diagrams/gov-tla/B1-constitution-2026.11.25.svg)**: is a similar, toy project using TLA+ to model the US Constitution and Government.

#### Writing

[The Gripping Hand](https://grippinghand.dev/): thesis, antithesis, synthesis.
