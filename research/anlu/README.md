# ANLU — Architecturally Native Language Understanding

**Research Lead:** Levario Ramirez  
**Status:** Track A complete (A0–A3). Track B in progress.  
**Core thesis:** Hallucination is a constraint problem. Give models physics and they behave like they live in a universe.

---

## The Primitive

> Geometry is information in boundary-surviving form. Constraints ARE information (Shannon).
> Frozen type embeddings introduce geometric impossibility — not just statistical unlikelihood.

All ANLU work encodes structure geometrically so it survives singularities. This is the load-bearing insight across the entire research program.

---

## Track A — Foundations (Complete)

| Paper | Title | Status |
|-------|-------|--------|
| A0 | Typed Embeddings: A Geometric Prior for Language Models | Complete |
| A1 | Typed Loops: Computational Depth as an Independent Improvement Axis | Complete |
| A2 | Learned Heuristics: Statistical Improvement Without Architectural Change | Complete |
| A3 | Epistemic Independence: Separating Knowledge from Reasoning | Complete |

**Orthogonality thesis (A0–A3 combined):** Pedagogy (training data order), frozen type embeddings (geometric priors), and loops (computational depth) are three orthogonal improvement axes operating in different mathematical categories — statistical, geometric/topological, and computational. A 2×2×2 factorial design proves non-interference.

---

## Track B — Constraint as Architecture (In Progress)

| Paper | Title | Status |
|-------|-------|--------|
| B1 | Hierarchy of Controls: A Safety Framework for LLM Architecture | Draft complete |
| B2 | Constraint as Information: The Shannon Bridge | Next |
| B3 | Alignment as Topology | Planned |

**Key external validation:** Bochkov (TMLR 2025) — frozen embeddings outperform trainable ones due to "representational interference." This is the strongest external confirmation of ANLU's geometric prior thesis and must be cited in B2.

---

## Publication Targets

- Track A: arXiv preprint bundle
- Track B: Conference track (NeurIPS / ICLR submission pending B3)
- Combined: Journal version for JMLR or TMLR

---

## Related Projects

- **ChatDB** — produces geometrically structured training data that matches ANLU's architecture
- **ProveCalc** — demonstrates constraint-as-information in engineering domain
- Both systems are empirical validation environments for the co-design principle
