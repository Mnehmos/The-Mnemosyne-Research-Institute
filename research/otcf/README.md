# OTCF — Oracle Trust Calibration Framework

**Research Lead:** Levario Ramirez  
**Status:** Active — gauntlet running, findings publishable  
**Platform:** LLM Chess Arena (TypeScript/Vite/Tauri)  
**Blog:** Mnehmos Astro blog (src/content/blog/ + src/pages/blog/)

---

## What It Is

The Oracle Trust Calibration Framework pits frontier LLMs against Stockfish at various ELO ratings under controlled experimental conditions. The goal: measure how, when, and why LLMs fail at chess — and use those failure modes as proxies for general cognitive failure patterns.

Chess is the benchmark because:
- Ground truth is computable (Stockfish eval)
- Move legality is binary (no partial credit)
- Cognitive load is tunable (ELO bracket)
- Failure modes are observable and categorizable

---

## Platform Architecture

**Four-voice architecture** (unique vs all known competitors):
1. **Player voice** — LLM reasoning trace
2. **Advisor voice** — Stockfish analysis
3. **Oracle/commentator voice** — Post-move evaluation
4. **Dead air filler** — Lichess puzzle solving during long think times

**Features:**
- P0–P6 prompt density spectrum (controls how much chess context the LLM receives)
- Live Twitch streaming with overlay
- Replay mode for historical games
- Benchmark data pipeline (Elo, win rates, centipawn loss)

---

## Published Findings

### Cognitive Failure Modes (5 identified)

1. **Forced-move blindness** — LLMs fail to find the only legal response when in check
2. **Endgame collapse** — Tactical strength drops sharply when piece count falls below threshold
3. **The Gemini Paradox** — Same model, same day: tactical brilliance vs. complete endgame collapse. Demonstrates within-session variance as a research finding
4. **Nemotron forced-move blindness** — Model-specific pattern: consistently misses forced responses
5. **Context saturation degradation** — Performance degrades as prompt length increases, even with relevant context

### Key Empirical Results

- Personal milestone: Vario broke 500 rapid on Chess.com during active research
- Gemini paradox documented with game records
- Nemotron blindness pattern reproducible across multiple sessions

---

## Next Features

- Real-time tournament commentary via Lichess broadcast API
- Expanded model coverage (targeting all frontier models)
- Publication to r/LocalLLaMA and Astro blog

---

## ChessReplay Component Note

The Mnehmos Astro blog uses a dual content pattern:
- Markdown posts: `src/content/blog/`
- Standalone pages: `src/pages/blog/`

ChessReplay component requires unique `id` props to avoid DOM collision when multiple games appear on one page.
