# AGENTS.md

This public repository distributes Burn release metadata and assets. Every commit is public immediately.

## Public Release Boundaries

- Commit only public release material. Never commit source code, build scripts, internal documentation, credentials, tokens, endpoints, or personal contact details.
- Give each release exactly one asset named `Burn-<version>.zip` and plain release notes.
- Publish releases only through the controlled release script. Never manually create releases or tags, upload or replace assets, attach a second asset, or change which release is latest. Release-note typo corrections are allowed.
- Never delete, rename, or replace a published `Burn-<version>.zip`; the updater requires that exact name. Ship rollbacks as a new, higher version.
- Limit hand edits to `README.md` and `icon.png`, accurate to the shipped app, and deliver them directly to `main`.

## Issue Tracking

- GitHub Issues are disabled. Do not create a local task queue, worklog, or changelog here.
