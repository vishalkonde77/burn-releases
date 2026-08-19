# How to Work in This Repo

This is the public, source-free distribution repository for Burn, a private macOS menu bar app. It exists so the app has somewhere public to fetch updates from. The source, docs, and build system live in a private repository; this repo is a downstream artifact of that one, and the private repository's instructions win on any conflict.

Everything here is public the moment it lands. Every rule below follows from that.

## What Lives Here

- `README.md`, the public-facing page for people installing Burn.
- `icon.png`, the image the README shows.
- GitHub Releases, one per version, each carrying exactly one asset named `Burn-<version>.zip` plus plain release notes.

Nothing else belongs here.

## Rules

- Never commit or upload source code, build scripts, internal docs, credentials, tokens, endpoints, or anything describing the private repository's contents. Never name or link the private repository; the README says the source is private and stops there.
- Releases are published only by the private repository's release script. Never create a release, upload an asset, attach a second asset, or re-tag anything by hand from this side.
- Never delete, rename, or replace a published `Burn-<version>.zip`. The app's built-in updater checks this repository daily, matches that exact asset name, and installs only a newer, correctly signed build; removing an asset breaks updates for anyone on that path. Correcting typos in release note text is fine.
- Never mark an older release as latest. The updater only moves forward; a rollback ships as a new, higher version, from the private side.
- Hand edits here are limited to `README.md` and `icon.png`, kept honest against what the shipped app actually does, and they go straight to `main`; a two-file repo has nothing worth branching for.

This repo deliberately has no worklog, changelog, or other working files. It is a distribution surface, not a project; the project's records live with the source.
