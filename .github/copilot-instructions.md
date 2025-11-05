<!--
Guidance for AI coding agents working in this repository.
This file is intentionally short and specific — prefer small, reviewable changes.
-->

# Copilot instructions — Mastikica

This repository is a personal GitHub profile repository. There is currently no application code, CI, or tests — only `README.md`. Keep changes minimal and make proposals via pull requests.

Key points for an AI coding agent:

- Big picture: This repo is a profile README. There are no services, build steps, or runtime components to modify. Any change should be straight-forward content edits, small assets, or adding a new project subfolder with its own README and manifest.

- Safe edits: When editing `README.md` prefer small, explicit updates. The repository contains a commented template block in the README (HTML comment). If you remove or replace it, explain why in the PR description and keep changes focused on content (no large refactors).

- No build/test commands: There is no package manifest or build system present. Do not add complex build tooling unless the user asks for a new project. If adding a project, include a minimal manifest (e.g., `package.json` or `pyproject.toml`) and a short README describing how to run and test it.

- Branching & PRs: Create a feature branch with a descriptive name (e.g., `feat/readme-update`), keep commits small and focused, and open a PR against `main`. In the PR description, include a short summary and any manual verification steps.

- Commit message conventions: Use imperative, concise messages (e.g., `docs: update README profile blurb`). Prefer separate commits for unrelated changes.

- When to ask the human: If a change touches anything beyond cosmetic README edits (new service, CI, infra, credentials, or external integrations), stop and ask for requirements or permission.

- Examples of acceptable actions without asking:
  - Fix typos or grammar in `README.md`.
  - Replace or reformat the profile template text for clarity.
  - Add a small image asset (under an `assets/` folder) referenced from the README.

- Examples of actions that require confirmation:
  - Adding CI workflows, Dockerfiles, or publishing scripts.
  - Creating a new service or launching infrastructure.
  - Adding third-party dependencies or secret-handling code.

- Files and patterns to reference:
  - `README.md` — primary content to edit.
  - `.github/` — create PR templates or workflows only with explicit user request.

If anything in this guidance is unclear or you need access to more context (owner intent, preferred biography text, or permitted contribution types), ask a human before making large changes.

When you've made a change, open a PR and include these items in the description:
- Short summary of what changed and why.
- Files modified and verification steps (what to look for in the rendered README).

Thank you — keep edits small, explicit, and reviewable.
