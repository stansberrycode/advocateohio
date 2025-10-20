## Purpose

This file gives short, actionable guidance for AI coding agents that will work on the `advocateohio` repository.

## Quick repository snapshot (discoverable facts)
- Current repository contains only a top-level `README.md` with project title.
- No source directories (src/, app/, api/), no language-specific manifests (package.json, pyproject.toml), and no CI config were found in the default branch.

## How to be immediately productive
- Start by noting the repo is effectively empty. Before making large changes, confirm the intended stack with the human owner (ask which language, framework, and CI they expect).
- Useful quick checks to run (mention these files/paths when making suggestions):
  - `README.md` — update with project description, stack, and dev setup.
  - `.github/` — add CI workflows if requested (e.g., GitHub Actions YAMLs).
  - `src/` or `app/` — typical default source folders depending on stack.

## Common tasks an AI agent can perform here
- Initialize a minimal project scaffold after confirming the stack. Examples:
  - For Node.js: create `package.json`, `src/index.js`, basic test with `npm test`.
  - For Python: create `pyproject.toml` or `requirements.txt`, `src/__init__.py`, and a pytest test.
- Create a short CONTRIBUTING.md or expand `README.md` with exact commands to build/test/run.
- Add a small GitHub Actions workflow under `.github/workflows/ci.yml` that runs lint + tests for the chosen stack.

## Patterns and conventions (what we could deduce)
- No project-specific conventions are discoverable yet. Treat repository structure and conventions as undefined until the owner provides them.

## Practical merging guidance (if this file already exists in other branches)
- Preserve any human-written sections in existing `.github/copilot-instructions.md` and append a short "Repo snapshot" block describing missing files.

## Examples to reference in suggestions
- When suggesting changes, reference `README.md` (present) and explicitly call out missing files (e.g., "no package.json found").

## What to ask the human owner first
1. Preferred language and framework (Node/Python/Ruby/etc.).
2. Preferred test runner and CI (Jest/pytest/GHA/CircleCI).
3. Any existing infra or external services to integrate (databases, auth, cloud provider).

## Safety and scope
- Do not add production-grade infra or push secrets. Propose examples and small scaffolds only; request permission before creating integrations or adding credentials.

---
If any section is unclear or you want the file tailored to a particular stack (Node, Python, Rails), tell me which stack and I'll update the instructions and add a minimal scaffold.
