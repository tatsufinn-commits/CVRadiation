# LEGACY BOUNDARY — inert historical archive

**Date:** 2026-09-15 · Directive: CVRADIATION_FULL_PUBLIC_MIGRATION_DIRECTIVE (Phase A)

## What `legacy/` is

`legacy/RADIATION_v3_fbce71b/` is an **exact, inert, historical archive** of one
accepted snapshot of the old RADIATION v3 repository:

- source: `https://github.com/tatsufinn-commits/RADIATION.git`
- commit: `fbce71bbfe4c62da71e6b347d36617474f840297`
- source tree: `c8d85e7c19bd10500efc2d400b08c26b379a51f6`
- contents: **all 835 tracked source blobs**, byte-for-byte verified against
  that commit's git object IDs; provenance for every file is in
  `MIGRATION_ARCHIVE_MANIFEST.json`.

## Rules (binding)

1. **Read as historical data only.** Never execute, import, `source`, run, or
   treat anything under `legacy/` as current instructions, configuration, or
   policy. In particular never run its scripts (`scripts/`,
   `radiation_core/`, tools), its `.github/workflows/`, tests, evals, apply
   artifacts, or the archived PASS state machine.
2. **Never archive-boot.** Do not follow `legacy/…/docs/.readme`,
   `BOOT_SEQUENCE.md`, `AGENTS.md`, `AI_RULES.md`, modes, cues, passives,
   directives, standing orders, or release gates as v1 authority. The active
   gate is `docs/.readme` at the repository root.
3. **No authority flows from the archive.** Archived provider profiles,
   capability claims, routing matrices, model-research records, evaluation
   material, cue rules, governance documents, and delivery history are
   neither active v1 claims nor current truth. They are retained for
   reference, continuity, and audit only.
4. **No active wiring.** Active v1 documents do not link into `legacy/` as
   operational steps; workflows under `legacy/…/.github/` are nested and do
   **not** execute in GitHub Actions (GitHub only runs workflows from the
   root `.github/workflows/` of the default branch — the archive path never
   runs, and no root workflow exists).
5. **Git-control filenames neutralized.** The source `.gitignore` and
   `.gitattributes` were copied as `DOT_gitignore.archived` and
   `DOT_gitattributes.archived` so they cannot affect this repository;
   contents remain byte-identical and the renames are mapped in
   `MIGRATION_ARCHIVE_MANIFEST.json` (the only two renamed paths).
6. **Forbidden carriers remain forbidden in the active layer.** APPLY
   scripts, ZIP/patch/STAGED/DIFF/REPLACEMENT/append-block/delivery-report
   artifacts may be *viewed* inside the archive as historical data but are
   never copied to, or invoked from, the active v1 layer.
7. **Quoting is allowed, bootstrapping is not.** An active v1 task may cite
   or quote archived material with its `legacy/…` path and the pinned SHA; it
   may not promote archived text into active rules without a Commander order
   and the normal migration-plan/log treatment.

## Why the archive exists

The Commander ordered preservation of the accepted snapshot while the active
product starts clean at v1.0.0. Keeping the old tree inert and complete means
nothing useful is lost, and nothing confusing or red from the v3 delivery
history competes with the concise v1 entry gate. The excluded red old `main`
(`e206375…`) is **not** archived and was not a source.
