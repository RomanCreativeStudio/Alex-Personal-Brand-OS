# Capture Workflow

Commands (`CAPTURE`, `STORY`, `EPISODE`, `LESSON`, `UPDATE OS`, `REVISE`) are
defined in `SYSTEM/CAPTURE_PROTOCOL.md`. This file defines the end-to-end
workflow, record format, and the ChatGPT/Claude contracts around it.

## Loop

```
CONVERSATION → CAPTURE → CLASSIFY → STORE → DEVELOP → PUBLISH → RESULT → REVISE
```

## Steps

1. Alex talks/asks/experiences something.
2. ChatGPT identifies potential signal — not every conversation.
3. ChatGPT outputs a compact `CAPTURE` record (see Record Format below).
4. Alex approves or rejects it.
5. Claude stores the approved record in `CONTENT/CAPTURES.md`.
6. Claude updates `CONTENT/IDEAS.md`, `QUESTIONS.md`, `LESSONS.md`, or
   `EPISODES.md` only when appropriate, and STORY/SERIES files only when the
   capture materially changes them.
7. The item can later become an episode (`EPISODE` command).
8. Published results can be added later (RESULT).
9. New information can trigger `REVISE` — history is preserved, not overwritten.

## What Gets Captured

Only: meaningful questions, real experiences, lessons, decisions, turning
points, useful observations, business/building moments, genuine story
developments. Not every conversation becomes a capture.

## Capture Record Format

```
ID:
DATE:
SOURCE:
TYPE:
CORE IDEA:
WHY IT MATTERS:
POTENTIAL CONTENT:
RELATED SERIES:
STATUS:
```

Optional (only when useful): `HOOK:`, `AUDIENCE:`, `NEXT STEP:`

## Status Values

`CAPTURED` · `REVIEW` · `IDEA` · `DEVELOPING` · `READY` · `PUBLISHED` ·
`REVISE` · `PRIVATE` · `ARCHIVED`

## ChatGPT Output Contract

When producing a `CAPTURE`, output only the compact record unless more
explanation is requested:

```
CAPTURE

ID: PBO-YYYY-MM-DD-###
DATE: YYYY-MM-DD
TYPE: ...
CORE IDEA: ...
WHY IT MATTERS: ...
POTENTIAL CONTENT: ...
RELATED SERIES: ...
STATUS: CAPTURED
```

## Claude Input Contract

On an approved `CAPTURE`:

1. Validate the record.
2. Assign/verify the ID.
3. Add it to `CONTENT/CAPTURES.md`.
4. Update `IDEAS.md` / `QUESTIONS.md` / `LESSONS.md` / `EPISODES.md` only
   when appropriate.
5. Update STORY/SERIES references only when the capture materially changes them.
6. Don't duplicate information unnecessarily.
7. Review `git diff`.
8. Commit only the relevant changes — `content: capture PBO-YYYY-MM-DD-###`.

## Not Yet Automated

This is a manual human/AI workflow — no APIs, webhooks, databases, agents,
scheduled jobs, GitHub Actions, or external integrations. Automation comes
after the workflow proves reliable.
