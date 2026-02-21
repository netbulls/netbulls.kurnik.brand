# Directory Boundaries

## Deploy directory
`site/` is the deployable static content directory. This is what gets served at brand.kurnik.ai.

- **DO NOT** use `docs/`, `public/`, `dist/`, or `out/`
- All HTML files intended for the live site go in `site/`
- Phase explorations: `site/phase-NN/round-NN-concepts.html`
- Phase documents: `site/phase-NN/index.html` or `site/phase-NN-name.html`

## Repo root
Keep clean. Only: `CLAUDE.md`, `CHANGELOG.md`, `README.md`, `.gitignore`, `.claude/`, `site/`, `deploy/`

## Large files
HTML files >50kb must be pushed via local git — the GitHub API truncates large content. Never attempt to push large files through the MCP GitHub tool.
