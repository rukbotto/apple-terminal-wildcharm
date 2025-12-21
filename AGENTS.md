# Repository Guidelines

## Project Structure & Module Organization
This repository is a single-purpose artifact repo that stores a macOS Terminal profile. The primary asset is `Wildcharm.terminal` at the repo root. There is no source code tree, build output directory, or test suite at this time. If new assets are added (e.g., alternate profiles or screenshots), keep them grouped at the root with clear names, or create a dedicated `assets/` directory and document it here.

## Build, Test, and Development Commands
There are currently no build or test scripts in this repository. Typical usage is manual import into Terminal:
- Open `Wildcharm.terminal` in Finder or run `open Wildcharm.terminal` to import the profile.
If you add automation (e.g., a script that generates profiles), list the exact command and what it produces.

## Coding Style & Naming Conventions
No codebase exists yet, so there are no formatting or linting tools configured. For new files:
- Use clear, descriptive filenames (e.g., `Wildcharm.terminal`, `Wildcharm-light.terminal`).
- Prefer ASCII content and keep files in UTF-8.
- If you add scripts, include a brief header comment explaining usage and required dependencies.

## Testing Guidelines
There are no automated tests. For manual verification:
- Import the profile into Terminal.
- Validate ANSI colors using a simple color test script or a known palette preview.
- Confirm behavior in both light and dark system themes if the profile uses dynamic colors.

## Commit Guidelines
- Always check for staged files before performing a commit by using `git diff --cached`. If staged files are found, perform the commit automatically as-is using. If not, ask human teammates to manually stage files before proceeding.
- Commits: 50 chars max, focused, imperative mood (e.g., "Add Header table sorting").
    - Commit message should summarize the changes made to staged files.
    - Additional details should be added as a bullet point list.
- Branches: simple, without slash parts (e.g., "add-header-table-sorting").

## Pull Request Guidelines
- Keep PRs atomic; update docs (README.md/AGENTS.md) when behavior changes.
- Push any pending changes to upstream before creating the PR.
- Give PRs 70-character titles and use the following template for the body; the template should be saved into a markdown file called `PR.md` at the root of the repo; recreate it if it's already present; for each section, format each title as second level headings and its contents as bullet point lists:
    - Summary: clear description about the changes.
    - Why: the reasoning behind the changes.
    - Key Changes: a clear description of each important change.
        - If applicable, include screeshots/GIFs for UI changes.
        - If applicable, include mermaid diagrams to describe code structure, use case flow, data flows and/or logic sequences.
    - How to Test: the steps required to test the changes.
    - Risk / Impact: a description of the risks & impacts these changes bring to the existing product.
    - Notes: additional notes.
- Create PRs using `gh` command and pass it the generated `PR.md` file as the body.

## Agent Notes
Keep changes minimal and explicit. Do not introduce new tooling or dependencies without documenting rationale and usage in this file.
