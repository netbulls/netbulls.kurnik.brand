# Directory Boundaries

## Deploy directory
`site/` is the deployable static content directory. This is what gets served at brand.kurnik.ai.

- **DO NOT** use `docs/`, `public/`, `dist/`, or `out/`
- All HTML files intended for the live site go in `site/`
- Phase explorations: `site/phase-NN/round-NN-concepts.html`
- Phase documents: `site/phase-NN/index.html` or `site/phase-NN-name.html`

## Repo root
Keep clean. Only: `CLAUDE.md`, `CHANGELOG.md`, `README.md`, `.gitignore`, `.claude/`, `site/`, `deploy/`

## Phase structure
Every phase gets its own directory: `site/phase-NN/`
- Each phase MUST have an `index.html` that serves as a hub linking to all content within that phase
- The site root `index.html` links to `/phase-NN/` for navigation
- Phase content files live inside their phase directory
- Exception: `site/brand-foundation.html` is a legacy flat file (Phase 01 index links to it)

## Large files
HTML files >50kb must be pushed via local git — the GitHub API truncates large content. Never attempt to push large files through the MCP GitHub tool.
