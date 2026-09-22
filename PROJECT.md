# How this book is made

This file explains the production process behind *The Plain White T-Shirt*. The book is an open manuscript built in public with plain text, Git, GitHub, and AI assistance. The process is part of the lesson: the same loop that produces the book is the loop students learn to run on their own projects.

## The production loop

Every change, large or small, travels the same path:

1. **Issue** — Work begins as a GitHub issue. The issue states what should exist and why, before anyone writes a word.
2. **Branch** — One branch per issue, named `issue-N-short-name`. Work stays isolated until it is ready for review.
3. **Prompt** — AI may draft or modify material, always from a bounded task. The human supplies intent, vocabulary, and constraints.
4. **Review** — Read the diff before committing. AI output is a first draft, never a finished decision.
5. **Commit** — Atomic commits: one issue, one logical change. The message says what changed and references the issue, e.g. `Develop Chapter 1 into a full draft #3`.
6. **Push** — Publish the branch so the work is visible and recoverable.
7. **Pull request** — The PR body closes the issue (`Closes #N`). Reviewers comment on lines, request changes, or approve in the GitHub interface.
8. **Merge** — Merge only after review and passing checks.
9. **Verify** — Confirm the verification workflow passes and the published site reflects the change.

## The SDLC as a map

The project uses a lightweight software development life cycle, modified for a small book rather than a large system. The phases are a map, not a bureaucracy: most issues move through all of them in a single sitting.

| Phase | The question | Artifacts |
|---|---|---|
| Plan | What should exist, and why? | GitHub issues, this file, `EDITORIAL.md` |
| Design | What will it say, and how will it look? | Chapter outlines, examples, `docs/sources.md` |
| Build | Make the thing. | Markdown chapters, layout, CSS |
| Review | Is it true, clear, and well made? | Pull request review, fact-checks, CI verification |
| Launch | Ship it. | Merge to `main`, GitHub Pages publish |
| Reflect | What changed, and what did we learn? | Notes in PRs and issues, revisions to `EDITORIAL.md` |

Issues carry a `phase: *` label so the board shows where each piece of work sits in the cycle.

## Working agreements

- **Atomic commits connected to issues.** Every commit references its issue number; the verification workflow checks for this traceability.
- **One issue per branch.** No drive-by changes; scope stays visible.
- **AI assists, humans decide.** Automation handles fast, repeatable checks. Humans remain responsible for intent, judgment, truthfulness, and final editorial decisions.
- **Verify before claiming done.** A task is finished when the checks pass and the change is visible where readers will see it.
- **Recoverability through version control.** Any state of the book can be restored; experiment freely on branches.

## Where this came from

The loop is practiced first in the [IS 117 hands-on practical](https://github.com/kaw393939/is117_test), a guided 45–60 minute exercise that produces a mini textbook through five bounded, AI-assisted issues. This repository is the full-scale version: the same loop, run at book length, with partner review and a published site.
