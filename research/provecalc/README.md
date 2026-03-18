# ProveCalc — Engineering Calculation Platform

**Lead:** Levario Ramirez  
**Status:** Active hardening (v0.1.0) — PDF pipeline, persistence contract, step-by-step surfacing  
**Stack:** Tauri 2.x + React 19 + Rust + Python (SymPy + Pint)  
**Website:** https://provecalc.com  
**Contact:** contact@themnemosyneresearchinstitute.com

---

## What It Is

ProveCalc is a desktop engineering calculation platform where:

- **LLM proposes** structural edits (never computes)
- **Engine validates** via SymPy + Pint (the source of truth)
- **Every step is auditable** — equations are nodes with dependency tracking
- **Verification gates** check unit consistency, constraint satisfaction, numeric residual, and sanity

Positioned against PTC Mathcad: "Buy once, own forever. Your calculations. Your license."

---

## Research Connection

ProveCalc is the **empirical engineering domain validation** for ANLU's constraint-as-information thesis:

- Dimensional analysis enforces geometric constraints on quantities
- Verification gates are the "hierarchy of controls" applied to calculation
- The assumption ledger is an explicit epistemic state machine
- Every node has provenance, verification status, and dependency tracking

This is hallucination prevention applied to engineering math, not natural language.

---

## Platform Scale

- ~43,000 lines of code
- 3-process architecture: React frontend / Rust backend / Python sidecar
- 32 Tauri commands, 19 sidecar endpoints
- 8 node types with full TypeScript/Rust/Python type parity
- 4-gate verification with PE-stamp-ready audit trail
- 7 worksheet templates (structural, mechanical, electrical, general)

---

## Current Priorities

1. Native PDF report pipeline (Workstream 4)
2. Save/load persistence contract hardening (Workstream 2)
3. Step-by-step solving surfaced in UI and exports (Workstream 5)
4. Structural engineering vertical expansion (Workstream 6)

---

## Published Output

- Volvox interview S01E01 (Feb 3, 2026) — YouTube: jtNd8biTUmI
- ProveCalc shipped in ~36 days from first commit
- 816+ tests at ship
