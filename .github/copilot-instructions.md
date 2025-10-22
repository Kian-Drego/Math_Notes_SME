## Purpose

This repository is a collection of mathematics study notes and past-paper resources (PDFs and plain text links). There is no build, runtime, or automated test system — most files are PDFs stored under topic folders. The goal of this guidance is to help an AI coding agent be immediately productive when editing, adding, or organizing content.

## Quick repo facts

- Root index: `notes.txt` (contains external links and resources).
- Topic folders: `Hypothesis Testing/`, `Statistical Distributions/`, `Statistical Sampling & Estimation/`.
- File types present: primarily `.pdf` and plain text. Example files: `Hypothesis Testing.pdf`, `Poisson Distribution.pdf`, `Mathematics Paper 3 Topical.pdf`.
- Git: single branch `main`. No CI, build, or test configuration detected.

## What to do first (agent checklist)

1. Read `notes.txt` to see the external resources referenced.
2. Inspect the specific topic folder before changing files (filenames use spaces and human-readable titles).
3. Do not attempt to modify PDF content in-place; instead, add companion notes in Markdown in the same folder.

## Useful patterns and conventions (discoverable)

- Folders are organized by topic. Place new material inside the matching topic folder.
- Filenames use spaces and Title Case (e.g., `Poisson Distribution.pdf`). Preserve that style for new files.
- There is no existing metadata/front-matter convention present in the repository.

## Recommended agent actions (concrete examples)

- To add a summary of an existing PDF, create a Markdown file next to it with a matching name, e.g.

  - `Statistical Distributions/Poisson Distribution.pdf`
  - `Statistical Distributions/Poisson Distribution — Summary.md`

- To add a new topical note, create a single Markdown file inside the relevant folder, e.g.

  - `Hypothesis Testing/Normal-approximation-notes.md` (use hyphens or spaces consistently across new files).

- Update `notes.txt` when adding new external links or primary resource references.

## Git & developer workflow notes

- Typical operations are simple file edits and commits. Example PowerShell commands (run from the repo root):

```powershell
git add "Statistical Distributions/Poisson Distribution — Summary.md"
git commit -m "Add Poisson distribution summary"
git push origin main
```

- Because files are stored in OneDrive-synced folders, watch for sync conflicts and locked files when adding or editing large PDFs.

## Integration & external dependencies

- This repository currently contains only local documents and external links in `notes.txt`. There are no code libraries, package manifests, or API integrations to interact with.

## When to ask the human

- If you need a preferred file format (PDF edit vs. Markdown summary), ask: the repo has no existing policy.
- If creating many new notes, ask where to place an index or whether to introduce structured metadata (there is none currently).

## Examples from this repo to reference

- `notes.txt` — top-level link index (see root).
- `Hypothesis Testing/Hypothesis Testing.pdf` — example of a topic PDF.
- `Statistical Distributions/Poisson Distribution.pdf` — example content to summarize.

## Closing

If anything in this instruction is unclear or you want a different convention (front-matter, index format, or automated checks), tell me which direction to prefer and I will update this file.
