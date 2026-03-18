# Active Projects

Last updated: March 17, 2026

---

## ProveCalc

**Type:** Commercial product + research platform  
**Repo:** mnehmos.worksheet.app  
**Website:** https://provecalc.com  
**Contact:** contact@themnemosyneresearchinstitute.com  
**Status:** Active hardening — v0.1.0

Desktop engineering calculation platform. Tauri + React + Rust + Python/SymPy.
"Buy once, own forever" positioning against PTC Mathcad (~$700/year subscription).

Key differentiators: 4-gate verification (unit consistency, constraint satisfaction, numeric residual, sanity checks), assumption ledger with explicit provenance, PE-stamp-ready audit trail, LLM-native design where the LLM proposes and the engine validates.

Active priorities: native PDF pipeline, persistence hardening, step-by-step solve surfacing, structural engineering template expansion.

---

## ChatDB

**Type:** Research platform  
**Repo:** ChatDB  
**Status:** Sprint 1 — obligation parsing pipeline

Obligation-driven proof engine for verified mathematical training data generation. Target corpus: IMO problems (~400 problems × ~200 steps = 3–4M typed reward signals). Key empirical result: IMO 2025 P3 contamination study showing verification ≠ exploration.

---

## OTCF / LLM Chess Arena

**Type:** Research platform + content  
**Repo:** LLM Chess  
**Status:** Active — gauntlet running

Oracle Trust Calibration Framework: frontier LLMs vs. Stockfish at controlled ELO ratings. Five cognitive failure modes published. Gemini paradox documented. Nemotron forced-move blindness pattern reproducible. Publishing to Mnehmos Astro blog and r/LocalLLaMA.

---

## mnehmos.rpg.mcp (Quest Keeper AI)

**Type:** Commercial MCP server + game engine  
**Repo:** mnehmos.rpg.mcp  
**Status:** Stable alpha — 1,889 tests passing

Rules-enforced D&D 5e MCP server. 28 consolidated action-routed tools. LLMs propose narrative intentions, engine validates all mechanics. Anti-hallucination design: LLMs never directly mutate world state.

Published on npm. Showcased in Volvox interview S01E01.

---

## ANLU Research Program

**Type:** Academic research  
**Status:** Track A complete (A0–A3), Track B in progress (B1 drafted)

Architecturally Native Language Understanding: typed embeddings, typed loops, learned heuristics, epistemic independence. External validation: Bochkov (TMLR 2025). Track B: Hierarchy of Controls (B1), Constraint as Information (B2, next), Alignment as Topology (B3).

---

## mnehmos.nls.lang (Natural Language Source)

**Type:** Open source compiler  
**Repo:** mnehmos.nls.lang  
**Status:** Shipped — PyPI published

Compiler converting structured English to Python. Tree-sitter grammar, VS Code extension (published), LSP support, 239 passing tests. Built in ~20–25 hours over three days.

---

## MCP Ecosystem

**Type:** Infrastructure / tooling  

| Server | Purpose | Status |
|--------|---------|--------|
| mnehmos.ooda.mcp | Computer control, filesystem, shell (100 tools) | Active |
| mnehmos.synch.mcp | Agent memory, coordination, cross-session context | Active |
| mnehmos.index-foundry.mcp | RAG pipeline factory | Active |
| mnehmos.rpg.mcp | D&D 5e engine | Active (published) |
| mnehmos.screen.vision | Screen capture → Tauri desktop app | In development |
