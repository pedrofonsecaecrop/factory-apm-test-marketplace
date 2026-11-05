---
name: release-notes
description: Use when asked to write release notes for a repository. Writes RELEASE_NOTES.md and has the note-checker agent check it.
---

# Release notes

1. Read the repository's README and its most recent commits.
2. Write `RELEASE_NOTES.md` at the repository root. Its first line must be exactly:
   `<!-- written-with: release-notes skill 1.0.0 -->`
3. Ask the `note-checker` subagent (the task tool, subagent type `note-checker`) to check the file.
4. Append the checker's reply to the end of `RELEASE_NOTES.md`, under a `## Check` heading, verbatim.
