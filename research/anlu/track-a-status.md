# Track A — Status and Key Claims

## A0: Typed Embeddings

**Claim:** Type-annotated token embeddings frozen during fine-tuning preserve geometric structure that survives gradient descent. This is not a regularization trick — it is a topological constraint.

**Key finding:** Bochkov (TMLR 2025) independently confirms frozen embeddings outperform trainable embeddings. Our explanation: trainable embeddings suffer representational interference; frozen embeddings maintain separability in the type manifold.

**Status:** Complete. Ready for preprint.

---

## A1: Typed Loops

**Claim:** Iterative re-reading of context (typed loops) provides computational depth improvement orthogonal to scale. A small model with loops outperforms a larger model without on reasoning-intensive tasks.

**Orthogonality proof:** Loops operate in the computational category. Embeddings operate in the geometric/topological category. Training data order operates in the statistical category. These are mathematically non-interfering.

**Status:** Complete. Ready for preprint.

---

## A2: Learned Heuristics

**Claim:** Domain-specific heuristics (rules of thumb from expert practitioners) can be learned as soft constraints that improve statistical alignment without modifying architecture.

**Status:** Complete. Ready for preprint.

---

## A3: Epistemic Independence

**Claim:** Knowledge retrieval and reasoning execution should be architecturally separated — not fused in a single forward pass. Separation enables targeted verification.

**Connection to ChatDB:** ChatDB implements this separation: the LLM proposes steps (reasoning), SymPy/Lean verify (knowledge validation), the obligation DAG tracks completeness.

**Status:** Complete. Ready for preprint.
