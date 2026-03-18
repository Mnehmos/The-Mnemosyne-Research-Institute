# The Mnemosyne Research Institute

**Domain:** themnemosyneresearchinstitute.com  
**Founded:** March 9, 2026 — Safford, Arizona  
**Contact:** info@themnemosyneresearchinstitute.com  
**Research inquiries:** research@themnemosyneresearchinstitute.com

---

## Who We Are

The Mnemosyne Research Institute is an independent AI research organization focused on three interlocking problems: how language models represent knowledge geometrically, how to generate training data that is formally verified rather than merely plausible, and how to build engineering tools that embody these principles in practice.

Our work is driven by a single load-bearing insight:

> **Hallucination is a constraint problem. Give models physics and they behave like they live in a universe.**

We are not a university lab. We are not a startup. We are a research-first organization that ships working systems as empirical validation of theoretical claims.

---

## Research Programs

### ANLU — Architecturally Native Language Understanding

The foundational theory. Typed embeddings as geometric priors. Frozen type embeddings that introduce geometric impossibility — not just statistical unlikelihood. Three orthogonal improvement axes (statistical, geometric/topological, computational) that compose without interference.

Track A (A0–A3): Complete. Covers typed embeddings, typed loops, learned heuristics, and epistemic independence.  
Track B (B1–B3): In progress. Hierarchy of Controls (B1 drafted), Constraint as Information (B2 next), Alignment as Topology (B3 planned).

External validation: Bochkov (TMLR 2025) — frozen embeddings outperform trainable embeddings due to representational interference. ANLU provides the theoretical explanation.

→ [Research details](research/anlu/README.md)

---

### ChatDB — Verified Training Data at Scale

An autonomous proof engine targeting the IMO corpus. LLMs propose steps. SymPy and Lean verify. An obligation DAG tracks what remains to be proven. Gated conclusions prevent premature termination.

Key finding: 19/19 locally verified steps on IMO 2025 P3 still produced the wrong answer (c=3 instead of c=4). Verification is not exploration. The architectural fix — evidence accumulator, verdict-last challenger format, tautology gates — is now implemented.

Scale target: 3–4 million typed reward signals from the IMO corpus. These signals are geometrically structured to match ANLU's architecture. The training data and the model architecture speak the same typed geometry. This is the research moat.

DARPA CLARA TA1 abstract drafted. Pending SAM.gov UEI registration.

→ [Research details](research/chatdb/README.md)

---

### OTCF — Oracle Trust Calibration Framework

An empirical benchmark using chess as the measurement domain. Frontier LLMs play against Stockfish at controlled ELO ratings under a P0–P6 prompt density spectrum. Cognitive failure modes are observed, categorized, and published.

Five failure modes documented to date: forced-move blindness, endgame collapse, the Gemini paradox (same model, same day — brilliant then broken), Nemotron forced-move blindness, and context saturation degradation.

Published to Mnehmos Astro blog and r/LocalLLaMA. Ongoing.

→ [Research details](research/otcf/README.md)

---

## Products

### ProveCalc

An engineering calculation platform built on the same constraint-as-information principle that underlies ANLU. The LLM proposes. The engine (SymPy + Pint) validates. Every assumption is explicit. Every step is auditable. Every result has a verification gate.

Positioned against PTC Mathcad: perpetual license, dimensional analysis native, PE-stamp-ready audit trail.

**Website:** https://provecalc.com  
**Contact:** contact@themnemosyneresearchinstitute.com

→ [Project details](research/provecalc/README.md)

---

### mnehmos.rpg.mcp

A rules-enforced D&D 5e backend MCP server. 28 consolidated action-routed tools. 1,889 tests. LLMs propose narrative intentions; the engine validates all mechanics. The same anti-hallucination design principle applied to role-playing games.

Published on npm. Powers the Quest Keeper AI desktop application.

---

## Active Projects

→ [Full project list](projects/active.md)

---

## Contact

| Purpose | Address |
|---------|---------|
| General inquiries | info@themnemosyneresearchinstitute.com |
| Research collaboration | research@themnemosyneresearchinstitute.com |
| ProveCalc / product | contact@themnemosyneresearchinstitute.com |
| Security disclosures | security@themnemosyneresearchinstitute.com |
| Administrative | admin@themnemosyneresearchinstitute.com |

---

*The Mnemosyne Research Institute — Safford, Arizona*
