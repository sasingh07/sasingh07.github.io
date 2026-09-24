---
name: Jekyll audit tooling
description: Environment-specific distinction between similarly named Lighthouse tools when auditing static Jekyll sites.
---

For a static Jekyll portfolio in this Replit environment, the Nix package named `lighthouse` may install an unrelated CLI rather than Google's website auditing tool. Do not interpret that command's presence as evidence that web audits can run.

**Why:** The system tool accepted installation but rejected a website URL as an unrecognized subcommand. Google's Lighthouse CLI, when invoked non-interactively, also required `--no-enable-error-reporting` to avoid a first-run prompt failing in a closed terminal.

**How to apply:** For future static-site audits, identify the executable before running it. If a temporary npm-based Google Lighthouse is needed, remove its generated Node package files and dependencies afterward so a Jekyll-only repository stays Jekyll-only.