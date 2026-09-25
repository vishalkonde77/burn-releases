# AGENTS.md

This public repository distributes Burn release metadata and assets. Every commit is public immediately, and the private source repository's instructions win on any conflict. Claude Code and Codex both read this file; its terse style is not a model for replies.

## Public Release Boundaries

- Commit only public release material. Never commit source code, build scripts, internal documentation, credentials, tokens, endpoints, personal contact details, or anything describing the private repository's contents.
- Never name or link the private repository. The README says the source is private and stops there.
- Give each release exactly one asset named `Burn-<version>.zip` and plain release notes.
- Publish releases only through the controlled release script. Never manually create releases or tags, upload or replace assets, attach a second asset, or mark an older release latest. Release-note typo corrections are allowed.
- Never delete, rename, or replace a published `Burn-<version>.zip`; the updater requires that exact name. Ship rollbacks as a new, higher version.
- Limit hand edits to `README.md` and `icon.png`, accurate to the shipped app, and deliver them directly to `main`; this overrides the global branch and pull request sequence, because a repository this small has nothing worth branching for.

## Issue Tracking

- GitHub Issues are disabled. Do not create a local task queue, worklog, or changelog here; anything reported about Burn is recorded upstream with the source.
