# GH-600 Exam Prep

Interactive, browser-based study tools for the GitHub GH-600 (Agentic AI Developer) certification.

## What it does

A small static website — no build step, no backend, no external dependencies — that bundles three study tools behind a landing page:

- **Interactive Course** (`course.html`) — walkthroughs of the six exam domains with examples, code snippets, and progress tracking.
- **Study Game** (`game.html`) — gamified terminology drills with score, streaks, and domain-based leveling.
- **Practice Exams** (`exam.html`) — Pearson VUE-style practice exams with a timed mode, per-domain scoring, and answer explanations.

The landing page (`index.html`) shows an overall-readiness summary aggregated across the tools.

Exam domains covered:

1. Prepare Agent Architecture & SDLC Processes
2. Implement Tool Use & Environment Interaction
3. Manage Memory, State & Execution
4. Perform Evaluation, Error Analysis & Tuning
5. Orchestrate Multi-Agent Coordination
6. Implement Guardrails & Accountability

## Status

Working, self-contained study site. The questions and course material are author-written prep content, not official GitHub exam material.

## Run

It's plain HTML/CSS/JavaScript. Either open `index.html` directly in a browser, or serve the folder over a local static server, for example:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Notes / limitations

- Progress, scores, and exam state are stored in the browser via `localStorage` — they live on the device/browser you use and aren't synced anywhere.
- Content is independent study material and is not affiliated with or endorsed by GitHub.
