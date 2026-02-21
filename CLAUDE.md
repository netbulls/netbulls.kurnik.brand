# Kurnik Brand — CLAUDE.md

> **Do NOT run `/init` on this project** — it will overwrite these instructions.

## Session start

**Read these files before doing anything:**
1. `DECISIONS.md` — full brand history, rationale, and phase context
2. `.claude/rules/brand-rules.md` — strict mark constraints
3. `.claude/rules/directory-boundaries.md` — file conventions

If Redis MCP is available, also read key `current_session_reality` for live session state.

---

## What this repo is

Brand assets, design explorations, and the public-facing brand site for **Kurnik** — an AI-powered product incubator.

Deployed at: **brand.kurnik.ai** ← `site/` directory
Org: **netbulls** (never `erace`)

---

## Critical conventions

- Deploy directory is `site/` — not `docs/`, not `public/`
- Every milestone gets a `CHANGELOG.md` entry: ISO 8601 + timezone + location
- Large HTML files (>50kb) must be pushed via local git, NOT the GitHub API
- Phase explorations: `site/phase-NN/round-NN-concepts.html`
- Each round = one commit. Never leave exploration files local-only.

---

## Mark rules (strict — do not deviate)

- **Monochrome only** — `#d4840a` on `#0e0c0a`. No opacity tricks for color variation.
- **Abstract** — NOT chicken, rooster, egg, comb, feather. The name is an inside joke; the mark does not illustrate it.
- **Scalable** — must read at 32px. No detail that disappears small.
- **Sensibility** — Figma, Linear, Vercel. Infrastructure-feel. Confident, minimal.
- **Vary via** — stroke weight, fill vs outline, positive/negative space, geometry

## Colors
| Token | Hex |
|-------|-----|
| Background | `#0e0c0a` |
| Amber (mark) | `#d4840a` |
| Amber light | `#f5a623` |
| Text | `#e8ddd0` |

## Typography
DM Serif Display · Manrope · DM Mono

---

## Phase status

| Phase | Status | Output |
|-------|--------|--------|
| 01 Brand Foundation | ✅ Complete | `site/brand-foundation.html` |
| 02 Symbol Exploration | ✅ Complete (850 concepts → 6 finalists) | `site/phase-02/` |
| 03 Assessment + Refinement | 🔄 Starting | score finalists, pick winner |
| 04 Final mark | ⏳ | lockup, color system, usage rules |

**Phase 02 finalists (4 families, 6 symbols):**
- F20-R6-03, F20-R6-02 — Chevron Cascade (ascending momentum)
- H1519-R6-03 — Bracket Arrows (engineering precision)
- T110-R6-01, T110-R6-08 — Rotated Squares (architectural geometry)
- B25-R6-01 — Arrow Void (bold direction)

---

## File structure

```
site/
  index.html
  brand-foundation.html              # Phase 01
  phase-02/
    round-01-concepts.html           # R01: 90 concepts
    round-02-concepts.html           # R02: 270 concepts
    round-03-concepts.html           # R03: 60 refined
    round-04-concepts.html           # R04: 100 fresh
    round-05-iterations.html         # R05: 220 iterations
    round-06-refinements.html        # R06: 110 refinements
    iteration-review.html            # Deep feedback
    icon-preview.html                # App icon testing
    lockup-preview.html              # Lockup font pairing
    round-03/ through round-06/      # SVG files
CHANGELOG.md
DECISIONS.md                         # Full history and rationale
.claude/rules/
  brand-rules.md
  directory-boundaries.md
  workflow.md
```
