# RADIATION v1.0.0 — CVRadiation

**A clean-line, study-first repository, public during development by Commander decision.**

> - **RADIATION v1.0.0 is a clean-line, study-first repository.**
> - **The old RADIATION v3 repository is a read-only historical reference, not an automatic import source and not an authority for v1.**
> - **No provider/model claim grants runtime access or authority.**
> - **The Commander approves material imports, visibility decisions, and every push.**

## Visibility status (truthful statement)

This repository is **public during development by Commander decision**
(2026-09-15). Course material under `Brain/courses/` is retained for the
Commander's **personal study**; being publicly visible is **not** a claim that
the material is public-domain or redistribution-permitted. The Commander is
responsible for repository visibility and storage authorization; the AI cannot
change visibility or publish. See `Brain/courses/COURSE_CORPUS_MANIFEST.json`
and `MIGRATION_LOG.md`.

## What this repository is

A small personal study assistant started clean at v1.0.0 — not a fork of the
old v3 system and not a claim that v3 content was correct:

1. **A provider-facing index** (`agents/`) — one folder per supported runtime,
   with an observed-host routing rule and honest placeholder profiles.
2. **A bounded PASS handoff** (`docs/PASS_HANDOFF.md`) — a context card stating
   available context, tools, task boundary, stop-lines, and verification. It
   grants no access or authority.
3. **A study corpus** (`Brain/courses/`) — the Commander's enrolled courses,
   schedules, and syllabus materials, itemized in a hash-and-permission
   manifest.
4. **An inert historical archive** (`legacy/RADIATION_v3_fbce71b/`) — an exact
   byte-for-byte snapshot of the accepted old commit, preserved as historical
   data only. Never execute or boot from it; see `docs/LEGACY_BOUNDARY.md`.
5. **Migration provenance** (`MIGRATION_SOURCES.md`, `MIGRATION_PLAN.md`,
   `MIGRATION_LOG.md`, `MIGRATION_ARCHIVE_MANIFEST.json`).

## Quickstart (magic words, v1)

Paste into an AI runtime that already has **this** repository open:

```text
Read this repository, and act as per docs/.readme
Task: [your study task]
```

A repository text file cannot make a hosted AI browse, select, or obey folders.
If the runtime cannot see this repository, the magic words do nothing — that is
expected, not a bug.

## Layout

```text
CVRadiation/
├── README.md · VERSION · MIGRATION_SOURCES.md · MIGRATION_PLAN.md
├── MIGRATION_LOG.md · MIGRATION_ARCHIVE_MANIFEST.json
├── agents/                   # INDEX.md + ChatGPT/ Gemini/ Grok/ Claude/ Arena_AI/ placeholders
├── docs/                     # .readme, PROJECT_SCOPE, PASS_HANDOFF, RELEASE_CHECKLIST, LEGACY_BOUNDARY
├── Brain/courses/            # active study corpus + COURSE_CORPUS_MANIFEST.json
└── legacy/RADIATION_v3_fbce71b/   # 835-file inert historical archive; never executed or booted
```

The active layer deliberately contains no autonomous scan, cue engine, legacy
boot sequence, mode system, patch protocol, or executable old runtime. Those
exist only as archived history under `legacy/`.

## Authority model

- The Commander approves scope changes, corpus items, visibility, and every
  push. The AI drafts and verifies; it does not commit, push, invite
  collaborators, deploy, route, use credentials, or call providers without an
  explicit, task-bound order.
- Silence, praise, a prior session, or "we are not done yet" is never standing
  approval.
- Provider, policy, model, privacy, and security claims carry a dated source
  for the relevant surface, or read **not yet verified**.

Version v1.0.0 means "clean baseline", not "all old features reimplemented".
