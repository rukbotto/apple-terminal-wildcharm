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
- Commits: 50 chars max, focused, imperative mood (e.g., "Add Header table sorting").
    - Commit message should summarize the changes made to staged files.
    - Add three bullet points to give more context about the commit.
    - Keep each commit small and focused.
- Avoid creating feature branches for this repo. Commit directly to `master` branch.

## Agent Notes
Keep changes minimal and explicit. Do not introduce new tooling or dependencies without documenting rationale and usage in this file.
