# Contributing to the book

This guide describes how changes to *The Plain White T-Shirt* get made, alone or with a partner. The short version lives in [PROJECT.md](PROJECT.md); this file is the working detail.

## The loop

Every change travels the same path:

1. **Pick or file an issue.** Work that is not an issue yet does not start yet. Assign yourself so nobody duplicates the effort.
2. **Branch from `main`.** Name it `issue-N-short-name`, e.g. `issue-3-chapter-1-draft`.

   ```sh
   git checkout main && git pull
   git checkout -b issue-N-short-name
   ```

3. **Do the work.** AI may draft from a bounded prompt; you review, correct, and decide.
4. **Commit atomically.** One issue, one logical change. Reference the issue in the message:

   ```sh
   git add path/to/file
   git commit -m "Develop Chapter 1 into a full draft #3"
   ```

5. **Push and open a pull request.** The PR body includes `Closes #N` so merging closes the issue.
6. **Review in the GitHub interface.** A partner comments on lines, requests changes, or approves.
7. **Merge, then verify.** Confirm the **Verify book** workflow passes and the published site shows the change.
8. **Sync before the next task:** `git checkout main && git pull`.

## Reviewing a partner's work

A review is part of the writing, not a gate around it.

- **Be specific.** Comment on the line, quote the phrase, name the problem.
- **Be kind.** Address the text, not the person.
- **Be actionable.** End with what should change: "cite a source for this claim" beats "this is weak."
- **Request changes** when something is wrong or unverified. **Approve** when you would be comfortable reading it aloud to a reader.

## Merge conflicts

Conflicts are normal when two people touch a shared file such as `docs/index.md` or `docs/assets/book.css`:

```sh
git checkout main && git pull
git checkout issue-N-short-name
git merge main
# resolve the marked sections, then:
git add .
git commit -m "Merge main into issue-N-short-name #N"
git push
```

Resolve deliberately. Keep both good intentions where possible; ask your partner when you cannot tell which change should win.

## Working with AI

- Give AI **bounded tasks**: one file, one section, one defined change.
- **Read every diff** before staging. You are the editor; the model is a fast assistant.
- Humans remain responsible for intent, judgment, truthfulness, appropriateness, and final editorial decisions.
- **Verify** quotations, objects, and links before committing them. Never commit invented evidence or testimonials.
- Label invented brands and examples as invented, per `EDITORIAL.md`.

## Definition of done

A task is done when the pull request is merged, the issue is closed, the verification workflow is green, and the change is visible to readers on the published site.
