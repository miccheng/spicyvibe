# AGENTS.md

## What this repo is

- A Markdown-only tutorial: "Getting Started with Vibe Coding" for OpenCode V2 (see `README.md`).
- No package manifests, build, test, lint, typecheck, CI, or codegen exist. Do not invent commands. Check with `git ls-files` before assuming otherwise.

## Layout

- `README.md`: index of the exercises. Update it when exercises are added or renamed.
- `exercises/exercise1.md` to `exercise5.md`, `exercises/bonus.md`: the lessons. Images live in `exercises/images/` and are referenced relatively (`./images/...`).
- `gemini-planned-it.md` and `The Transition to Intent-First Coding.pdf` (root): reference material.

## Editing conventions

- Each exercise ends with a `[Next Exercise >>](./exerciseN.md)` link. Exercise 5 links to `./bonus.md`. Keep this chain intact when reordering or renaming.
- Exercises are step-by-step instructions for learners running commands in a terminal on macOS and Windows. Keep steps concrete and in order.
- Learner projects live in a `vibeprojects` folder on the learner's Desktop, outside this repo. Do not scaffold app code here unless asked.

## Git state

- The working tree may contain the user's uncommitted changes. At the time of writing: the PDF and `gemini-planned-it.md` are deleted, and `exercises/bonus.md` is modified. Do not restore, commit, or discard these unless the user asks.
- Commit subjects are short and imperative, for example "Fix typo and refer to 'Build Mode' explicitly."
