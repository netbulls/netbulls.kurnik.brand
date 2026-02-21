# DECISIONS.md

Full decision history for **netbulls.kurnik.brand** — the *why* behind brand choices. Written for Claude Code continuity. Read this before starting any brand session.

---

## 2026-02-21 · Warsaw, PL — Bootstrap session

### Name selection
Explored: Prism (too crowded, OpenAI conflict), Sift (taken), Glean ($7B company conflict), Kura (multiple conflicts).

**Final: Kurnik** — Polish for "chicken coop." Domain kurnik.ai registered. Inside joke — PlayOK (nostalgic Polish games site) is kurnik.pl. Memorable, warm, nobody in tech has it.

**Critical implication: the mark does NOT illustrate the name.** Chicken/rooster/egg/comb references explored in Phase 02 Round 01 and abandoned. The name is the joke. The mark stands alone.

### Audience
Primary: founders, aspiring entrepreneurs, people with capital but no methodology. NOT dev teams initially. Affects tone — approachable and credible, not technical.

### Personality
Warm & confident. Notion meets Stripe. Premium incubator feel. Not playful, not clinical.

### Color rationale
- Dark = premium, focused, serious (Linear, Vercel, Raycast)
- Amber = warmth, approachability — breaks the cold tech blue/purple cliché
- Stone scale for neutrals — warm undertone, not cold

Final tokens:
- `#0e0c0a` — near-black, warm undertone
- `#d4840a` — amber primary / mark color
- `#f5a623` — amber highlight
- `#e8ddd0` — warm off-white text
- `#2a2420` — border/divider

### Typography
DM Serif Display (display) + Manrope (UI) + DM Mono (code/labels). Warmth, distinctiveness, readability at small sizes.

---

## Phase 02 — Symbol exploration

### Round 01 (inconclusive)
- 90 SVG concepts across 4 territories: Geometric Rooster, Egg+Rooster Fusion, Comb/Crown, Nested/Negative Space
- None compelling. Territories too literal — forced chicken/rooster references.
- Lesson: don't illustrate the name.
- Semi-promising:
  - **A20** Circuit Rooster — systematic, constructed, engineered quality
  - **B13** Half Shell — arch + legs, architectural feel
  - **B10** Emergence — shape rising from base, upward energy
- Thread: **structured geometry with upward/emergent energy**

### Technical lesson from Round 01
Large HTML files (>50kb) must be pushed via local git. GitHub API truncates large content fields. All future rounds must be generated locally and pushed via `git push`.

### Monochrome rule — why
Established after Round 01 review. Opacity variations were creating false color variety, masking weak shapes. Strict monochrome forces the mark to work on geometry alone — which is the real test of a good logo.

### Round 02 direction
Six abstract territories, zero animal references:
1. **Upward / Emergence** — shapes rising from a base. Launch, growth, threshold.
2. **Contained / Portal** — shape within a shape. Negative space as subject.
3. **Systematic / Grid** — modular, engineered, precise. Circuits, lattices.
4. **Radial / Convergence** — elements from/toward center. Orbits, bursts.
5. **Letterform / Abstract K** — not a literal K. Distorted, fragmented, reconstructed.
6. **Tension / Duality** — two shapes in dialogue. Split forms, mirror structures.

### Sensibility reference
Figma, Linear, Vercel, Stripe. Infrastructure-feel. Confident, minimal, slightly cold. Not playful, not illustrative.

### Evaluation framework (100 points)
- Visual Design: 30pt
- Symbolic Meaning: 25pt
- Color Strategy: 20pt
- Typography-Icon Harmony: 15pt
- Audience Resonance: 10pt

---

## Phase structure

| Phase | Goal | Status |
|-------|------|--------|
| 01 | Brand Foundation document | ✅ Complete |
| 02 | 100+ symbol concepts, iterate to ~3 candidates | 🔄 Round 01 done, Round 02 next |
| 03 | Refine top 3 — weights, spacing, variants | ⏳ |
| 04 | Final mark — lockup, color system, usage rules | ⏳ |

## File organization

```
site/
  brand-foundation.html         # Phase 01 — live
  phase-02/
    round-01-concepts.html      # 90 concepts (inconclusive)
    round-02-concepts.html      # 120 concepts — next
    round-NN-concepts.html      # iterate until compelling candidates
  phase-03/
    ...                         # refinement of top candidates
```

Each round = one commit. Never leave exploration files uncommitted.
