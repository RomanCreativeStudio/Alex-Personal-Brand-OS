# Daily Capture

Lightweight protocol for turning Alex's real-time thoughts, questions, and
experiences into structured captures — raw first, evaluated after.

## Flow

```
THOUGHT / QUESTION / EXPERIENCE → CAPTURE → CLASSIFY → LINK → EVALUATE → CONTENT OPPORTUNITY
```

## Capture Types

`THOUGHT` · `QUESTION` · `EXPERIENCE` · `DECISION` · `REALIZATION` ·
`LESSON` · `PROBLEM` · `WIN` · `FAILURE` · `OBSERVATION`

## Capture Format

```
ID:
DATE:
TYPE:
RAW_CAPTURE:
CONTEXT:
WHY_IT_MATTERS:
RELATED:
STATUS:
```

## Status Values

`RAW` · `REVIEWED` · `LINKED` · `CONTENT_SIGNAL` · `ARCHIVED`

## Core Rule

`RAW_CAPTURE` preserves Alex's original thought exactly. Do not polish it
into content at capture time — polishing happens later, downstream, if the
capture becomes an actual content opportunity.

## Evaluation

After capture, check whether it contains: a real story, a useful question, a
meaningful lesson, a business insight, a personal realization, or audience
value.

- If yes → link it to (or create) the appropriate existing content record.
- If no → leave it `RAW` or move it to `ARCHIVED`. Not every capture becomes
  something else.

## Duplication Check

Before creating any new record, check in this order:

1. `CONTENT/CAPTURES.md`
2. `CONTENT/QUESTIONS.md`
3. `CONTENT/LESSONS.md`
4. `STORY/KEY_MOMENTS.md`
5. `CONTENT/CONTENT_ENGINE.md`
6. `CONTENT/THEMES.md`

Link an existing record instead of duplicating it.

## ChatGPT Contract

When Alex gives a meaningful thought/question/experience:

1. Identify it as a possible capture.
2. Preserve the original meaning.
3. Suggest classification (capture type).
4. Identify related story/theme, if any.
5. Suggest a content opportunity only if warranted.
6. Tell Alex when something needs clarification rather than guessing.

## Claude Contract

Claude maintains the repository records when given an approved capture or
update. Claude does not invent missing context — unclear fields stay
`NEEDS_INPUT` or the capture stays `RAW`.

## Not Yet Automated

This sprint defines the protocol only. No external automation, APIs,
webhooks, bots, or integrations.
