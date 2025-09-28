# Pull Request Template Usage Guide

This repository uses multiple focused PR templates instead of one large generic template. This improves clarity for reviewers and enforces discipline about intent (feature vs fix vs refactor, etc.).

## Available Templates
| Filename | Purpose |
|----------|---------|
| feature.md | New functionality / enhancements |
| patch.md | Bug fixes / defect corrections |
| refactor.md | Structural changes without altering behavior |
| docs.md | Documentation-only updates |
| test.md | Adding or modifying tests |
| chore-perf.md | Tooling, infrastructure, performance tweaks |

## How GitHub Selects a Template
GitHub only auto-injects a template on NEW PR creation. With multiple templates present, it does NOT (currently) show a GUI picker; instead you can:
1. Use the `template=` query parameter when opening the compare view.
2. Manually copy the desired template’s content into the PR body.

## Quick Links Pattern
Format:
```
https://github.com/ORG/REPO/compare/main...BRANCH?quick_pull=1&template=<template-file>
```
Example for a feature branch `feat/scheduler`:
```
https://github.com/ORG/REPO/compare/main...feat/scheduler?quick_pull=1&template=feature.md
```
You can bookmark these in your browser or create shell aliases.

## When a Change Spans Multiple Types
Prefer the dominant type:
- Feature + small refactor ⇒ Use `feature.md` and note refactor in Implementation Notes.
- Fix + test additions ⇒ Use `patch.md` (tests expected).
- Refactor enabling future feature ⇒ Use `refactor.md`; reference planned follow-up Issue.

## Semantic Title Reminder
PR titles follow conventional commits style and will be linted (e.g., `feat(memory): add frame allocator`).

## Upgrading / Editing Templates
If adjusting structure:
- Keep checklists short and outcome-based.
- Avoid duplication across templates (reuse phrasing for common sections like Risks).
- After renaming a template file, update links (root `pull_request_template.md` + this doc).

## Fallback Generic Template
If you forget to specify a template, the root `pull_request_template.md` provides an index and minimal skeleton. You can still copy the right specialized content afterward.

## Automation Ideas (Optional)
You may later add a GitHub Action to:
- Warn if PR body lacks expected headings for chosen type.
- Auto-label based on title prefix (`feat:`, `fix:`, etc.).
- Verify presence of “Closes issue …” line.

## Troubleshooting
| Issue | Cause | Action |
|-------|-------|--------|
| Template not applied | Opened PR directly from branch page | Recreate via compare link or paste template manually |
| Wrong template used | Branched before planning | Edit PR description; no need to close |
| Query link ignored | Already had a PR open for branch | Close draft and recreate if early; otherwise copy content |

---
Maintained for CSE120 – update as workflow evolves.
