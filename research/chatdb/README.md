# ChatDB — Obligation-Driven Proof Engine

**Research Lead:** Levario Ramirez  
**Status:** Sprint 1 active — obligation parsing pipeline  
**Stack:** Tauri (Rust) + React + Python sidecar (SymPy + Lean)  

---

## What It Is

ChatDB is an autonomous proof engine that generates verified mathematical training data. Unlike existing math LLM tools, ChatDB implements a strict separation:

- **LLM proposes** proof steps (never computes)
- **SymPy/Lean verify** each step before it's accepted
- **Obligation DAG** tracks what still needs to be proven
- **GATED conclusions** prevent premature termination

The target corpus is IMO (International Math Olympiad) problems. Scale: ~400 problems × ~200 verified steps × multiple attempts × 6–8 signals = **3–4 million typed reward signals** in a typed graph structure.

---

## Core Design

The database is the intelligence. Every step, decision, and verdict is recorded in SQLite. The system is deterministic and auditable.

**Architecture layers:**
- Rust orchestrates (hot path, IPC, document model)
- Python validates (SymPy symbolic math, Lean formal verification)
- React observes (never mutates state directly)
- Frontend listens to Tauri events

---

## Key Empirical Finding

**IMO 2025 Problem 3 contamination study:**

19/19 locally verified steps yielded the wrong answer (c=3 instead of c=4). "Verification is not exploration." Multiple frontier models converged on c=3/2 due to training prior contamination.

Architectural fixes implemented:
- Evidence accumulator
- Verdict-last challenger format
- Tautology gates


---

## The Co-Design Moat

ChatDB and ProveCalc both produce geometrically structured data that matches ANLU's geometrically structured architecture. Data types, model types, and frozen anchors speak the same typed geometry. This is the research moat:

> "Hallucination is a constraint problem. Give models physics and they behave like they live in a universe."

---

## Current Sprint

Sprint 1 critical path:
1. Fix DAG foundation bugs (parent_ids always None)
2. Layer 1: Solver self-tagging JSON sidecar
3. Layer 4: Validator-generated obligations
4. Layer 3: Classifier ensemble (2–3 models parallel)
5. Merge pipeline with dedup and confidence scoring
6. Pre-solve intelligence briefing (4 parallel agents)
7. Wire all 3 layers via `tokio::join!`
