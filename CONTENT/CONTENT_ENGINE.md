# Content Engine v1

Turns verified captures, questions, stories, lessons, and themes into
structured content opportunities. Source records are referenced by ID, not
duplicated — see the linked files for full content.

```
CAPTURE → STORY / QUESTION / LESSON → THEME → ANGLE → EPISODE → CONTENT
```

## Inputs

`CAPTURE` (`CONTENT/CAPTURES.md`) · `QUESTION` (`CONTENT/QUESTIONS.md`) ·
`STORY` (`STORY/KEY_MOMENTS.md`) · `LESSON` (`CONTENT/LESSONS.md`) ·
`THEME` (`CONTENT/THEMES.md`)

## Process

1. Identify source record(s).
2. Identify audience/problem.
3. Identify lesson/value.
4. Select content angle.
5. Decide best format.
6. Link to series.
7. Assign status.

## Content Opportunity Format

```
ID:
SOURCE:
THEME:
CORE IDEA:
LESSON:
AUDIENCE:
ANGLE:
FORMAT:
SERIES:
STATUS:
```

**FORMAT options:** `SHORT_VIDEO` · `LONG_VIDEO` · `CAROUSEL` · `TEXT_POST` · `STORY` · `EPISODE`
**STATUS values:** `SIGNAL` · `IDEA` · `READY` · `PUBLISHED` · `REVISE`

**Question rule:** a question becomes an opportunity only if it contains a
useful problem, realization, decision, or lesson.
**Story rule:** story comes before content — never reverse-engineer a fake
story from a content idea.
**Episode rule:** only create an episode when the source has enough
substance; not to pad the count.
**Linking rule:** every opportunity must point to at least one source ID.

---

## Opportunities

### CO-001

**SOURCE:** `PBO-2026-08-13-001`, `S-2026-08-13-001`
**THEME:** `T-001`
**CORE IDEA:** Using ChatGPT and Claude extensively surfaced friction that contributed to wanting to build AIMA.
**LESSON:** NEEDS_INPUT — no formal LESSON record tied to this capture yet (only the STORY/INTERPRETATION note on `S-2026-08-13-001`).
**AUDIENCE:** NEEDS_INPUT — not yet defined anywhere in the repo.
**ANGLE:** "Two AI Tools Helped Me Realize I Needed to Build a Third." (existing concept — not a finalized title)
**FORMAT:** EPISODE — see `EP-CONCEPT-001` in `CONTENT/EPISODES.md` (concept only, not duplicated here)
**SERIES:** AIMA, THE_BUILD
**STATUS:** IDEA
**PLATFORM VERSIONS:** `FMT-001`, `FMT-002`, `FMT-003` in `CONTENT/FORMATS.md`

### CO-002

**SOURCE:** `Q-2026-08-13-001`, `L-2026-08-13-001`
**THEME:** `T-002`
**CORE IDEA:** Building a personal brand system that documents real life instead of manufacturing content.
**LESSON:** `L-2026-08-13-001` — document the life you're actually building; don't manufacture one for content.
**AUDIENCE:** NEEDS_INPUT
**ANGLE:** Why I'm documenting my actual life instead of manufacturing content for a brand. (derived directly from `L-2026-08-13-001`)
**FORMAT:** TEXT_POST
**SERIES:** THE_JOURNEY, REAL_LIFE
**STATUS:** IDEA
**PLATFORM VERSIONS:** `FMT-004`, `FMT-005` in `CONTENT/FORMATS.md`

---

## Themes Not Yet Developed

- **T-003** (Builder Identity) — only declarative `MASTER_STORY.md` statements exist, no specific captured moment/question/lesson. Not enough substance for an opportunity yet — would be reverse-engineering a story from a theme.
- **T-004** (RCS — The Agency Build) — existence only, no client work, decisions, or moments captured. Same reasoning.

No new CAPTURE, QUESTION, STORY, or LESSON records were created or modified
in this pass.
