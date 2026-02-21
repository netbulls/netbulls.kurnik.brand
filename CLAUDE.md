# Kurnik Brand — CLAUDE.md

## What this repo is

Brand assets, design explorations, and the public-facing brand site for **Kurnik** — an AI-powered product incubator.

Deployed at: **brand.kurnik.ai** ← `site/` directory  
Org: **netbulls** (never `erace`)

---

## Critical conventions

- Deploy directory is `site/` — not `docs/`, not `public/`
- Every milestone gets a `CHANGELOG.md` entry: ISO 8601 + timezone + location
  - Example: `2026-02-21T18:00:00+01:00 · Warsaw, PL`
- Large HTML files (>50kb) must be pushed via script, not the GitHub API directly
- Phase explorations live at `site/phase-NN/round-NN-concepts.html`

---

## Brand foundation

**Name:** Kurnik — Polish for "chicken coop." Inside joke. The mark does NOT illustrate this.

**Personality:** Warm & confident. Notion meets Stripe. Premium incubator feel.

**Colors:**
- Background: `#0e0c0a`
- Accent / mark color: `#d4840a` (amber)
- Text: `#e8ddd0`

**Mark rules (strict):**
- Monochrome only — `#d4840a` on dark. No multi-color, no opacity tricks for color variation.
- Abstract, timeless, infrastructure-feel — think Figma, Linear, Vercel
- NOT chicken, rooster, egg, comb, or feather references
- Must read at 32px. No decorative detail that disappears small.
- Vary via: stroke weight, fill vs outline, positive/negative space, geometry

---

## Phase status

### Phase 01 — Brand Foundation ✅
- Brand Foundation document: `site/brand-foundation.html`
- Live at brand.kurnik.ai/brand-foundation.html

### Phase 02 — Symbol Exploration 🔄
- Round 01: `site/phase-02/round-01-concepts.html` — 90 concepts, 4 territories. None compelling.
- Round 02+: 120 concepts, 6 territories (see below), done in local code due to file size.

**Round 02 territories:**
1. Upward / Emergence — shapes rising from a base
2. Contained / Portal — negative space as subject
3. Systematic / Grid — modular, engineered, precise
4. Radial / Convergence — elements emanating from/toward center
5. Letterform / Abstract K — not a literal K, distorted/reconstructed
6. Tension / Duality — two shapes in dialogue

**Semi-promising from R01:** A20 (constructed/systematic), B13 (arch structure), B10 (emergence)

### Phase 03 — Refinement ⏳
Top candidates from Phase 02 → 3 refined directions → scoring

### Phase 04 — Final mark ⏳
Selected direction → lockup → color system → usage rules

---

## File structure

```
site/
  index.html                    # Brand site landing
  brand-foundation.html         # Phase 01 document
  phase-02/
    round-01-concepts.html      # 90 SVG concepts (R01)
    round-02-concepts.html      # 120 SVG concepts (R02) ← next
    round-NN-concepts.html      # future rounds
  phase-03/
    ...
CHANGELOG.md
README.md
deploy/                         # deploy scripts
```

---

## Pushing large files

Files >50kb must be pushed via local git or a script — the GitHub API truncates large `content` fields.

```bash
git add site/phase-02/round-02-concepts.html
git commit -m "Phase 02 Round 02 — 120 SVG concepts, 6 territories"
git push
```
