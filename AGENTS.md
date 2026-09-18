# Agent Guide

## Project

- Repository: `ortnit/sudoku`
- Purpose: small Python Sudoku solver.

## Source-derived documentation governance

Python code, tests, lock and manifest files, and examples are authoritative for current executable behavior, Python requirements, dependencies, and verification commands. Documentation records intent, decisions, constraints, and links to authoritative artifacts.

Before adding prose, make the derivability decision:

> Can a fresh agent derive this statement reliably from code, tests, lock files, or configuration?

- If yes, improve names or contracts if needed, then link to the authoritative artifact instead of paraphrasing it.
- If no, record the non-derivable intent, rationale, invariant, risk, or human procedure in the correct document.

Do not add ADR, PRD, glossary, runbook, ownership, or generator structures unless this repository has real content for them. Keep this project small; prefer clearer code and tests over explanatory prose.

## Working rules

- Read this file, `CLAUDE.md`, relevant docs, and current `git status` before editing.
- Keep changes small and scoped. Remove in-scope duplicated prose rather than synchronizing another copy.
- Keep the solver small and understandable.
- Do not install dependencies, release, or inspect secrets unless explicitly delegated.
- After verified task-scoped changes, commit and push directly in small, traceable commits when the repository has a safe upstream.
- Verify with repository-native checks and `git diff --check` before handoff.
