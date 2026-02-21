# Workflow Rules

## Every iteration gets committed
Each round of brand exploration (SVG concepts, type tests, lockup attempts) gets its own commit to the brand repo. No orphaned local files.

## Naming convention
- Phase explorations: `site/phase-NN/round-NN-concepts.html`
- Phase documents (published): `site/phase-NN-[name].html` or `site/phase-NN/index.html`

## CHANGELOG on milestones
Update `CHANGELOG.md` when:
- A phase is complete
- A direction is locked/rejected
- A significant decision is made

Format: `YYYY-MM-DDTHH:MM:SS+HH:MM · City, Country`

## Do not push secrets
No API keys, credentials, or tokens. Brand repo is public.
