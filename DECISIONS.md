# DECISIONS.md

Full decision history for **netbulls.kurnik.brand** — the *why* behind brand choices. Written for Claude Code continuity. Read this before starting any brand session.

---

## 2026-02-21 · Warsaw, PL — Bootstrap session

### Name selection
Explored: Prism (too crowded, OpenAI conflict), Sift (taken), Glean ($7B company conflict), Kura (multiple conflicts).

**Final: Kurnik** — Polish for "chicken coop." Domain kurnik.ai registered. This is an inside joke — PlayOK (nostalgic Polish games site) is kurnik.pl. The name is memorable, warm, nobody in tech has it.

**Critical implication: the mark does NOT illustrate the name.** Chicken/rooster/egg/comb references were explored in Phase 02 Round 01 and abandoned. The name is the inside joke. The mark needs to stand alone as abstract, timeless, infrastructure-feel.

### Audience
Primary: founders, aspiring entrepreneurs, people with capital but no methodology. NOT dev teams initially. This affects tone — approachable and credible, not technical.

### Personality
Warm & confident. Notion meets Stripe. Premium incubator feel. Not playful, not clinical.

### Color rationale
Dark backgrounds + warm amber accents chosen deliberately:
- Dark = premium, focused, serious (like Linear, Vercel, Raycast)
- Amber = warmth, approachability, breaks the "cold tech" cliché of blue/purple
- Stone scale for neutrals (not pure black/grey — too harsh)

Final tokens:
- `#0e0c0a` — near-black background (warm undertone, not cold)
- `#d4840a` — amber primary
- `#f5a623` — amber highlight
- `#e8ddd0` — warm off-white text

### Typography
DM Serif Display (display) + Manrope (UI) + DM Mono (code/labels). Chosen for: warmth, distinctiveness, readability at small sizes.

---

## Phase 02 — Symbol exploration

### Round 01 (inconclusive)
- 90 SVG concepts across 4 territories: Geometric Rooster, Egg+Rooster Fusion, Comb/Crown, Nested/Negative Space
- None were compelling. Territories too literal — forced chicken/rooster references.
- Lesson: don't illustrate the name. The mark needs to transcend the inside joke.
- Semi-promising concepts:
  - **A20** (Circuit Rooster) — liked the systematic, constructed, engineered quality
  - **B13** (Half Shell) — arch + legs structure, architectural feel
  - **B10** (Emergence) — shape rising from a base, upward energy
- Thread across all three: **structured geometry with upward/emergent energy**

### Round 01 — technical lesson
Large HTML files (>50kb) must be pushed via local git. GitHub API truncates large content fields. Round 02+ must be generated in local code and pushed via `git push`.

### Round 02 direction
Six abstract territories, no animal references:
1. **Upward / Emergence** — shapes rising from a base. Launch, growth, threshold.
2. **Contained / Portal** — shape within a shape. Negative space as subject.
3. **Systematic / Grid** — modular, engineered, precise. Circuits, lattices.
4. **Radial / Convergence** — elements from/toward a center. Orbits, bursts.
5. **Letterform / Abstract K** — not a literal K. Distorted, fragmented, reconstructed.
6. **Tension / Duality** — two shapes in dialogue. Split forms, mirror structures.

### Monochrome rule (strict)
Established after Round 01 review. Opacity variations were creating false color variety.
- **Only** `#d4840a` on `#0e0c0a`
- No opacity tricks for color variation
- Contrast and hierarchy via: stroke weight, fill vs outline, positive/negative space, geometry
- Must read at 32px

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
| 02 | Symbol exploration — 100+ concepts, iterate to ~3 candidates | 🔄 Round 01 done, Round 02 next |
| 03 | Refine top 3 candidates — weights, spacing, variants | ⏳ Pending |
| 04 | Final mark — lockup, color system, usage rules | ⏳ Pending |

## File organization

```
site/
  brand-foundation.html      # Phase 01 — live
  phase-02/
    round-01-concepts.html   # 90 concepts (inconclusive)
    round-02-concepts.html   # 120 concepts — next
    round-NN-concepts.html   # iterate until compelling candidates emerge
  phase-03/
    ...                      # refinement of top candidates
```

Each round = one commit. Never leave exploration files uncommitted.
