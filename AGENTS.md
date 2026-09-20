# Burn Public Releases Instructions

This public repository distributes Burn release metadata and assets. Everything committed here is public immediately.

## Public Release Boundaries

- Keep only public release material here. Never commit source code, build scripts, internal documentation, credentials, tokens, endpoints, or personal contact details.
- Each release has exactly one asset named `Burn-<version>.zip` and plain release notes.
- Only the controlled release script publishes a release. Do not manually create releases or tags, upload or replace assets, attach a second asset, or change which release is latest. Release-note typo corrections are allowed.
- Do not delete, rename, or replace a published `Burn-<version>.zip`; the updater needs that exact asset name. A rollback ships as a new, higher version.
- Hand edits are limited to `README.md` and `icon.png`, kept accurate to the shipped app, and go directly to `main`.

## Issue Tracking

- GitHub Issues are intentionally disabled. Do not create a local task queue, worklog, or changelog here.
