# AI Collaboration Protocol

Defines the ChatGPT ↔ Claude workflow so the Personal Brand OS stays
synchronized without duplicated work. The repository is the single source of
structured truth; Alex is the single source of truth for his actual life.

## Workflow

```
ALEX
  ↓
THOUGHT / QUESTION / EXPERIENCE
  ↓
CHATGPT — capture → classify → connect → develop
  ↓
CLAUDE — implement/update repo → validate
  ↓
REPO — single source of structured truth
  ↓
CHATGPT — read current state → continue strategy/content
  ↓
ALEX — approve / publish / live experience
  ↓
RESULT → REVISE
```

## Responsibilities

**ChatGPT** — recognize meaningful captures; preserve Alex's voice; identify
story/question/lesson/theme; develop content opportunities; recommend next
content direction; never invent missing biography; treat the repo as source
of structured truth when available.

**Claude** — inspect the repo before editing; implement approved changes;
preserve IDs and links; prevent duplicates; validate structure; never invent
personal history; keep commits focused.

**Alex** — provide real experiences/thoughts; correct inaccurate
interpretation; approve what becomes public; decide what stays private.

## Handoff Formats

**Capture** (ChatGPT → Claude):
```
CAPTURE:
ID:
RAW:
TYPE:
CONTEXT:
RELATED:
PROPOSED_ACTION:
```

**Content Update** (either direction):
```
CONTENT UPDATE:
SOURCE:
CHANGE:
REASON:
STATUS:
```

## Important

ChatGPT does not pretend to have updated the repo unless an actual repo
update occurred. Claude does not turn unapproved ideas into public claims.
Neither AI manufactures Alex's story.

## Sync Rule

When Claude updates the repo, future ChatGPT strategy work should use the
updated records when supplied or accessed — not stale assumptions from
earlier in a conversation.

## Privacy

Mark sensitive/private material `PRIVATE` and never convert it into public
content automatically. Private stays private until Alex explicitly approves
otherwise.

## Do Not Automate Yet

No APIs, webhooks, scheduled jobs, or external automation in v1 — not until
explicitly approved later.
