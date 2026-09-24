# CLAUDE.md (burn-releases)

This is Burn's public, source-free release repository. Everything committed here is public immediately, and the private source repository's instructions win on any conflict.

## What Lives Here

- The working tree holds only `CLAUDE.md`, `AGENTS.md`, `README.md`, and the `icon.png` it shows.
- Each version ships as one GitHub Release carrying exactly one asset named `Burn-<version>.zip` plus plain release notes.

## Rules

- Never commit or upload source code, build scripts, internal docs, credentials, tokens, endpoints, anything describing the private repository's contents, or anyone's name or contact details beyond the account that owns this repository.
- Never name or link the private repository. The README says the source is private and stops there.
- Releases are published only by the private repository's release script, so never create a release, upload an asset, attach a second asset, or re-tag anything by hand here.
- Never delete, rename, or replace a published `Burn-<version>.zip`, because the app's updater matches that exact asset name and removing one breaks updates in progress. Correcting typos in release note text is fine.
- Never mark an older release as latest. The updater only moves forward, and a rollback ships from the private side as a new, higher version.
- Hand edits are limited to `README.md` and `icon.png`, kept honest against what the shipped app actually does, and they go straight to `main`. This overrides the global branch and pull request sequence, because a repository this small has nothing worth branching for.
- This repository keeps no worklog, changelog, or task queue, and GitHub Issues are switched off on purpose, so the `file-issue` skill cannot run here. That overrides the global rules on keeping repository documents current and on Issues being the only queue.
- Anything reported about Burn is recorded upstream with the source, never on this side.
