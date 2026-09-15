# PROJECT SCOPE — RADIATION v1.0.0

**Date:** 2026-09-15 · **Status:** Commander-approved baseline (decision D3)

## Purpose

RADIATION v1 is a practical, **private, study-first** study-assistant
repository for the Commander's enrolled courses. It exists to:

- hold the Commander's course digests, syllabi, calendars, and schedules;
- answer, organize, and drill study questions from that corpus on demand;
- maintain an honest, source-dated provider-facing index;
- make every session's access, tools, and limits explicit via the PASS card.

## In scope for v1.0.0

| Capability | Surface |
|---|---|
| Study support from corpus derivatives | `Brain/courses/` (manifest-declared, on demand) |
| Provider routing honesty | `agents/INDEX.md`, five placeholder provider READMEs |
| Context handoff | `docs/PASS_HANDOFF.md` |
| Release discipline | `docs/RELEASE_CHECKLIST.md` |
| Provenance | `MIGRATION_SOURCES.md`, `MIGRATION_PLAN.md`, `MIGRATION_LOG.md` |

## Out of scope for v1.0.0 (excluded or deferred)

- **No autonomous runtime.** No autopilot, modes, standing directives, standing
  orders, autonomous patch/cue engine, or self-directed writes (v3 cue/,
  subskills/, AI_RULES/MODES machinery excluded — M-057/M-060/M-061).
- **No model decisions.** No routing matrix, model-evaluation results,
  automatic model selection, deployment configuration, or external-provider
  calls (M-011, M-053/M-056, M-057). The model-research catalog is deferred by
  Commander decision D5.
- **No governance apparatus.** No control-plane relay, task receipts/evidence
  bundles, validators, shrine, or patch-ledger workflow (M-057/M-058/M-061).
- **No redistribution.** The study corpus stays private; third-party school
  assets are never republished (M-027…M-033).
- **No credential handling.** Calendar feeds are stored data; feed secrets and
  tokens stay out of the tree. CI with credentials is excluded (M-057).
- **No legal/compliance conclusions.** Provider policy notes are dated research
  or say "not yet verified"; nothing here is a legal opinion.

## Corpus boundary

- `Brain/courses/` contains only manifest-declared files, loaded on demand.
- Every file binds path, sha256, media type, role, privacy classification,
  source (pinned blob SHA for imports), and the Commander approval reference.
- Markdown derivatives are the normal AI-readable layer; source binaries
  (PDF/DOCX/HTML) are fidelity sources loaded only when explicitly tasked.
- `desktop.ini`-style environment clutter is not imported (M-034).
- Additions need a Commander order, a manifest row, and a log row.

## Authority model

- The Commander approves scope changes, every corpus item, and every push.
- The AI drafts, verifies, and reports; it never commits, pushes, invites,
  deploys, routes, or uses credentials without a task-bound order.
- Positive feedback is not ratification; silence is not expanded authority; a
  local permission is not a standing order; "not done" is not permission to
  build.
- Source discipline: claims carry a dated primary/source for the relevant
  surface, or read **not yet verified**. See `agents/INDEX.md` for the
  evidence-tier method retained from the old research layer.

## What "v1.0.0" means

A clean, understandable baseline — not a re-implementation of v3 and not a
claim that old v3 content was correct. Later work resumes one bounded task at a
time (study support, observed PASS behavior, dated profile refreshes, and only
then anything larger), each with its own Commander order.
