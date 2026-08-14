# Question → Content Engine

Core principle: **every question is a signal; not every question is content.**
Approved question signals are stored in `CONTENT/QUESTIONS.md`. This file
defines how a question gets evaluated and, if warranted, developed.

## Pipeline

```
QUESTION → CONTEXT → WHY IT MATTERS → STORY → LESSON → CONTENT ANGLE → EPISODE → PUBLISH → RESULT → REVISE
```

## Question Record

```
QUESTION ID:
DATE:
QUESTION:
CONTEXT:
SIGNAL:
TYPE:
POTENTIAL LESSON:
CONTENT ANGLE:
RELATED SERIES:
STATUS:
```

Optional (only when useful): `HOOK:`, `EPISODE:`, `RELATED CAPTURE:`

## Question Types

`DECISION` · `PROBLEM` · `LESSON` · `BELIEF` · `REALIZATION` · `BUSINESS` ·
`BUILDING` · `AIMA` · `RCS` · `FAITH` · `PERSONAL GROWTH` · `TECHNICAL` · `FUTURE`

## Signal Test

A question becomes a content candidate when at least one is true:

1. Alex has personally experienced the problem.
2. Alex is actively trying to solve it.
3. Alex learned something meaningful from it.
4. The question represents a turning point.
5. The question exposes an authentic tension.
6. Other people likely face the same problem.
7. The answer connects to Alex's journey.
8. The answer could teach something useful.

If none apply: `STATUS: PRIVATE` or `STATUS: ARCHIVED`. Do not force content.

## Story First

Prefer developing content as:

```
WHAT HAPPENED → WHAT ALEX THOUGHT → WHAT ALEX DID → WHAT HAPPENED NEXT → WHAT HE LEARNED → WHAT SOMEONE ELSE CAN LEARN
```

Avoid generic advice disconnected from Alex's actual experience.

## Example (illustrative only — not a real project record)

> Q: "Should I focus on RCS, AIMA, or the client meeting tonight?"
> Signal: DECISION / BUSINESS / BUILDING
> Lesson: Building multiple things requires deciding what deserves attention
> now rather than working on everything.
> Content angle: "The hardest part of building isn't knowing what to do. It's
> knowing what NOT to do."
> Status: IDEA

## Content Development

A question may produce a story, a lesson, an episode, a series entry, or
multiple future ideas — choose the smallest useful output. Do not
automatically generate all of them.

## Episode & Capture Connections

- If a question has enough context to become an episode, reference it by ID
  in `CONTENT/EPISODES.md` (no full script in this sprint — idea architecture only).
- Questions can reference existing entries in `CONTENT/CAPTURES.md` by ID.
  Never duplicate the full capture.

## Series Connections

A question may belong to one or more of: `THE_BUILD`, `THE_JOURNEY`, `RCS`,
`AIMA`, `FAITH`, `WHAT_IM_LEARNING`, `REAL_LIFE`. Assign only the relevant ones.

## ChatGPT Contract

When a strong question-based content opportunity is identified, output only
the compact record unless more explanation is requested:

```
QUESTION SIGNAL

ID: Q-YYYY-MM-DD-###
QUESTION: ...
CONTEXT: ...
SIGNAL: ...
TYPE: ...
POTENTIAL LESSON: ...
CONTENT ANGLE: ...
RELATED SERIES: ...
STATUS: IDEA
```

## Claude Contract

On an approved `QUESTION SIGNAL`:

1. Validate it.
2. Assign/verify the ID.
3. Add it to `CONTENT/QUESTIONS.md`.
4. Link existing captures where appropriate (by ID, no duplication).
5. Link an episode only if one already exists.
6. Do not invent context.
7. Do not duplicate information.
8. Review `git diff`.
9. Commit only the relevant changes.

## Not Yet Automated

No API integrations, webhooks, databases, AI agents, scheduled jobs, GitHub
Actions, or external services. This workflow must prove itself manually first.
