<div align="justify">

### Scott Cochran

I work on AI Safety using formal methods, policy as code, and assisted development.

I use AI to make AI safer and easier to work with.

</div>

<table>
<tr>
<td width="50%" valign="top">
<div align="justify">

#### Agentic AI, safe by design

- **[TOPAK](https://github.com/scottcochran/TOPAK)** is an architecture pattern for "Safe by Design" agentic AI collaboration. It treats every agent as Byzantine and keeps models out of the trusted computing base using [TLA+, OPA, Cedar, and Paxos](https://grippinghand.dev/topak).
  
  - TLA+ specs and proofs, using mutations, witnesses and hypothesis flipping
  - A policy floor in Cedar, narrowed per request by an OPA/Rego bundle that can deny but never grant
  - Multi-Paxos ordering the control-plane log; Kafka as transport only
  - A Rust reference implementation of the admit path, with its admit decision proved in Lean 4
  - Agent orchestration via promoted workflows and a tree of narrowing control planes (Proposed)

</div>
</td>
<td width="50%" valign="top">
<div align="justify">

#### TLA+

- **[tla-kit](https://github.com/scottcochran/tla-kit)**: the TLA+ tools in one container image, with an MCP server for agents. Docker is the only dependency.

  - TLC, SANY, PlusCal and TLAPS with Z3, Zenon, Isabelle and LS4, every tool held to a sha256 digest
  - Reproducible builds: base image by digest, packages from a dated Ubuntu snapshot, attested releases
  - 14 MCP tools: parse, symbols, evaluate, TLC runs, simulation, coverage, state graphs, proofs, flip tests and proof sync
  - `prove` by theorem, step or line, reporting each failed obligation and why each backend failed
  - Paired with the [writing-tla-specs-and-proofs](https://github.com/scottcochran/TOPAK/tree/main/skills/writing-tla-specs-and-proofs) plugin; the same setup runs locally and in GitHub Actions
  - `tla-kit-selftest` checks the image against itself in about 30 seconds

</div>
</td>
</tr>
</table>

<table>
<tr>
<td colspan="2" valign="top">
<div align="justify">

#### Proof posters

These are click-navigable posters of Lean and TLA proofs. They adapt to light and dark themes, are pinned to source, and reproducibly generated. Each one is released by version tag with checksums.

</div>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<div align="justify">

- **[riemann-diagrams](https://scottcochran.github.io/riemann-diagrams/)**: twenty posters of the theorem
dependency graph of Alpöge's Lean proof of the Riemann Hypothesis. They show the proof [chapter by chapter](https://scottcochran.github.io/riemann-diagrams/diagrams/R2-chapters-2026.11.23.svg), [single
chains](https://scottcochran.github.io/riemann-diagrams/diagrams/T2-trace-landau-2026.11.23.svg) of [reductions](https://scottcochran.github.io/riemann-diagrams/diagrams/T1-trace-deepest-2026.11.23.svg), its [definitions](https://scottcochran.github.io/riemann-diagrams/diagrams/R1-main-theorems-2026.11.23.svg), its [literature](https://scottcochran.github.io/riemann-diagrams/diagrams/F4-literature-2026.11.23.svg), and [what's "new"](https://scottcochran.github.io/riemann-diagrams/diagrams/F2-new-2026.11.23.svg).

- **[riemann-masullo-diagrams](https://scottcochran.github.io/riemann-masullo-diagrams/)**: posters of the
riemann-masullo Lean formalisation of A. M. Masullo's *The Music of the Primes*. They show what in it rests on
the [steps no one knows how to repair](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M2-no-repair-2026.11.25.svg): the [cone of each open step](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M2-no-repair-2026.11.25.svg), the [paper by depth below its target theorems](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M3-depth-2026.11.25.svg),
and the [printed claims the Lean refutes](https://scottcochran.github.io/riemann-masullo-diagrams/diagrams/M5-refuted-2026.11.25.svg).

- **[TOPAK](https://scottcochran.github.io/TOPAK/)**: fifty-eight posters of the TOPAK architecture, drawn from
its decision records, specs and checkpoints. They show the [roles](https://scottcochran.github.io/TOPAK/diagrams/topak/A1-roles-map-2026.10.05.svg),
the [authority chain](https://scottcochran.github.io/TOPAK/diagrams/topak/B1-authority-chain-2026.10.05.svg) from intent to effect,
the [admit pipeline](https://scottcochran.github.io/TOPAK/diagrams/topak/D1-admit-pipeline-2026.10.05.svg),
the [trusted base](https://scottcochran.github.io/TOPAK/diagrams/topak/G1-trusted-base-2026.10.05.svg),
[every check and proof](https://scottcochran.github.io/TOPAK/diagrams/topak/H3-verification-map-2026.10.05.svg),
and [the premises each theorem rests on](https://scottcochran.github.io/TOPAK/diagrams/topak/G3-theorem-premise-dag-2026.10.05.svg).
Every record, file and name in them links to its source at a pinned commit.

</div>
</td>
<td width="50%" valign="top">
<div align="justify">

- **[anthropic-vp-vnp](https://scottcochran.github.io/anthropic-vp-vnp/)**: posters of *VP ≠ VNP over every field*
and its Lean 4 formalization in [anthropics/formal-math](https://github.com/anthropics/formal-math/tree/main/vp-vnp).
They show the proof [section by section](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/R2-sections-2026.11.25.svg),
[the route to the main theorems](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/R3-route-2026.11.25.svg),
[the paper against the Lean](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/F1-paper-lean-2026.11.25.svg),
and the paper's own [Figure 1, checked](https://scottcochran.github.io/anthropic-vp-vnp/diagrams/F4-figure-1-2026.11.25.svg)
arrow by arrow against the Lean.

- [proof-posters](https://github.com/scottcochran/riemann-diagrams/tree/main/plugins/proof-posters) is my Claude Code plugin which was used to build the posters.

- **[gov-tla](https://scottcochran.github.io/gov-tla/diagrams/gov-tla/B1-constitution-2026.11.25.svg)**: is a similar, toy project using TLA+ to model the US Constitution and Government.

</div>
</td>
</tr>
</table>

<table>
<tr>
<td valign="top">
<div align="justify">

#### Writing

[The Gripping Hand](https://grippinghand.dev/): thesis, antithesis, synthesis.

</div>
</td>
</tr>
</table>
