No source to build a soul from: `soul/SOUL.md`, `STYLE.md`, `examples/`, and `data/` are all untouched scaffold — no X handle, name, or links anywhere, and no `var` was passed in this run.

Per the skill's step 0, when no source resolves, the correct behavior is to skip cleanly with no notification (this isn't a failure, so nothing goes to `./notify`).

## Summary
- Checked `soul/SOUL.md`, `soul/STYLE.md`, `soul/examples/`, `soul/data/` — all scaffold, no handle/name/links to work from.
- Logged `SOUL_BUILDER_SKIP: no source — set var (x=, name=, or links=)` to `memory/logs/2026-07-27.md`.
- No notification sent (per skill spec for the no-source case).
- Follow-up: to build a soul, the operator needs to set `var` via the dashboard's "Build my soul" button (e.g. `x=handle`, `name=Full Name`, or `links=url1,url2`) and re-run this skill.
