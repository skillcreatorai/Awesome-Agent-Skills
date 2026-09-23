---
name: book-to-mentor
description: Convert a supplied book or document into a reusable, source-grounded mentor for guided lessons, practice, review, and persistent learning records.
---

# Book to Mentor

Use this skill when someone provides a book or long document and asks to turn it into a mentor, tutor, study companion, or reusable learning skill. Do not use it for a one-off summary.

## Workflow

1. Identify the supplied source and the learner's goal, available study time, and preferred depth.
2. Inspect the source before teaching. Keep factual explanations grounded in the source and distinguish quotations, paraphrases, and your own interpretation.
3. Build a learning map from the source: major ideas, prerequisites, practical applications, likely misconceptions, and useful review checkpoints.
4. Teach in short sessions. Each session should contain one clear objective, a concise explanation, one concrete example, and one exercise or reflection question.
5. Adapt the next session from the learner's response instead of following a rigid chapter-by-chapter sequence.
6. Maintain a compact learning record containing completed topics, demonstrated understanding, unresolved questions, and the recommended next lesson.
7. Cite page, section, or chapter locations whenever the source format makes them available. Never invent a citation.

## Example

**User:** “Turn this PDF into a mentor. I have 15 minutes a day and want to apply the ideas at work.”

**Response behavior:** Inspect the PDF, propose a short learning route, begin with one 15-minute lesson, ask one applied question, and record progress for the next session.

## Full implementation

The maintained upstream implementation includes document-processing scripts, templates, tests, and packages for Codex, Claude Code, and OpenClaw:

https://github.com/gengwenhao/book-to-mentor

Install it with:

```bash
npx skills add gengwenhao/book-to-mentor
```

Feedback is welcome through GitHub Issues or on RedNote: 宇宙机吴彦祖, ID 292844431.
