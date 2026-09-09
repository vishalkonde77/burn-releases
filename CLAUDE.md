# CLAUDE.md (burn-releases)

Working memory for agents in this repo: the conventions and pitfalls an agent cannot learn by reading it. The global instructions load alongside this file, and a rule here that deliberately differs from them is marked as an override with its reason. This is the public, source-free distribution repository for Burn, a private macOS menu bar app. Everything here is public the moment it lands. The source, docs, and build system live in a private repository whose instructions win on any conflict.

## What Lives Here

- The working tree holds only `CLAUDE.md`, `README.md`, and the `icon.png` it shows.
- Each version ships as one GitHub Release carrying exactly one asset named `Burn-<version>.zip` plus plain release notes.
- Nothing else belongs here, including a generated `AGENTS.md`, which would make a fourth file. `CLAUDE.md` is deliberately left out of the sync that creates one.

## Rules

- Never commit or upload source code, build scripts, internal docs, credentials, tokens, endpoints, anything describing the private repository's contents, or anyone's name or contact details beyond the account that owns this repository.
- Never name or link the private repository. The README says the source is private and stops there.
- Releases are published only by the private repository's release script, so never create a release, upload an asset, attach a second asset, or re-tag anything by hand here.
- Never delete, rename, or replace a published `Burn-<version>.zip`, because the app's updater matches that exact asset name and removing one breaks updates in progress. Correcting typos in release note text is fine.
- Never mark an older release as latest. The updater only moves forward, and a rollback ships from the private side as a new, higher version.
- Hand edits are limited to `README.md` and `icon.png`, kept honest against what the shipped app actually does, and they go straight to `main`. This overrides the global branch and pull request sequence, because a repository this small has nothing worth branching for.
- This repository keeps no worklog, changelog, or task queue, and GitHub Issues are switched off on purpose. That overrides the global rules on keeping repository documents current and on Issues being the only queue.
- Anything reported about Burn is recorded upstream with the source, never on this side.

<!-- agents-sync:end-shared -->

## Claude Code Specific

- The `file-issue` skill cannot run here, because Issues are disabled.
