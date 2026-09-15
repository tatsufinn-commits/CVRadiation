# MIGRATION SOURCES

Record of what the v1.0.0 migration may look at, what it may not use, and how
inspection was performed.

## 1. Safe source snapshot (the ONLY inspected snapshot)

| Field | Value |
|---|---|
| Old repository | https://github.com/tatsufinn-commits/RADIATION.git |
| Inspected commit SHA | `fbce71bbfe4c62da71e6b347d36617474f840297` |
| Commit tree SHA | `c8d85e7c19bd10500efc2d400b08c26b379a51f6` |
| Commit date | 2026-09-15T02:39:29Z |
| Commit message | "Repair public tree: remove stale superseded Fable record" |
| Snapshot size | 176 directories, 835 files (GitHub tree API, `recursive=1`, not truncated) |
| Plan date | 2026-09-15 (Asia/Singapore) |
| Status at acceptance | Last independently accepted clean snapshot for the stale Fable-record repair; 14 active model-research records; green structural baseline at that time |

The 14 model-research JSON records and the pinned tree's file inventory are
listed with blob SHAs in `MIGRATION_PLAN.md`.

## 2. Excluded pending separate repair acceptance

| Reference | Status | Treatment |
|---|---|---|
| Current old `main`, SHA `e206375783f13216ea9e73b78549517e21d42c09` | **Red as of 2026-09-15**; carries an unresolved accidental carrier/placeholder payload | **Not inspected, not copied**, neither as a tree nor as a version reference |
| Any v3 delivery report claiming something was "built" or "green" | Not public-state proof | Not used as an import source |
| Local candidates, ZIPs, named branches, prose reports | Not public-state proof | Not used |

The pinned snapshot is a point-in-time reference, not a claim that everything in
it is correct or wanted in v1. Each candidate is decided row-by-row in
`MIGRATION_PLAN.md`.

## 3. Other repository observed: `CVRadiation`

The Commander also asked the planner to read
https://github.com/tatsufinn-commits/CVRadiation. Observed 2026-09-15:

- **Public** repository (`"private": false` via GitHub API), created
  2026-09-15T04:31:31Z, single branch `main` at
  `a600a30ea3e9bb36fb32729da5ca7fc6fa80724b`, 50 files.
- Contents are an **early RADIATION v1.0.0-era scaffold** (four-mode README
  dated 2026-09-12, `PROTOCOL.md`, `BOOT_SEQUENCE.md`, `cue/`, `styles/`,
  `subskills/`, `scaffolding/`, a stub `Brain/`). It has **no `agents/`
  provider folders, no course corpus, and no model-research catalog**. Its
  quickstart text still points at the old RADIATION.git URL.
- It is **not named in the migration order as a source**, and it was not used as
  one. Whether it is the migration target (it would first have to be made
  private and its scaffold reconciled), a separate experiment, or irrelevant is
  a Commander decision — see `MIGRATION_PLAN.md` §8, decision D1.

## 4. How inspection was done (and what was never done)

- Read-only GitHub REST (`commits`, `git/trees`) and `raw.githubusercontent.com`
  fetches of the pinned SHA, performed from the migration workspace on
  2026-09-15. No clone, checkout, submodule, hook, or script run.
- Every source file was treated as **data**. Nothing in the old tree was
  executed, including `APPLY.sh`/`APPLY.ps1`, `radiation_pass.py`, validators,
  probes, or workflows. (The PASS script was read as text only, to understand
  the handoff concept for rewriting.)
- No file from any source has been copied into the v1 tree. The bootstrap files
  in this directory were handwritten for v1.
- One read-only, in-session host check: on 2026-09-15 `arena.ai/agent`,
  `arena.ai/privacy`, `arena.ai/terms`, and `arena.ai/pricing` returned HTTP
  200; the privacy/terms/pricing pages had been recorded as 404/reCAPTCHA in the
  old profiles (2026-09-14/15). Contents were not reviewed; this is logged as a
  changed-status review trigger, not a verified claim.
- The raw inspection cache (tree JSON and fetched source texts) is held OUTSIDE
  the v1 tree in the migration workspace under `.inspect/`; it is reference
  data, never to be committed, and may be deleted on order.

## 5. Phase 2 execution note (2026-09-15, after Commander approvals)

Approvals CMD-2026-09-15-D1…D6 are recorded in `MIGRATION_PLAN.md` §0. Under
those approvals the AI built the v1 tree **in the local workspace only**:

- handwritten framework: root `README.md`, `agents/` (INDEX + five placeholder
  provider READMEs), `docs/` (`.readme`, `PROJECT_SCOPE.md`, `PASS_HANDOFF.md`,
  `RELEASE_CHECKLIST.md`);
- 18 verbatim corpus files copied from the pinned snapshot into
  `Brain/courses/`, each verified byte-identical to its pinned git blob
  (SHA-1) and cross-checked by sha256; plus two rewritten course files
  (`INDEX.md`, `README.md`) and a rebaselined `COURSE_CORPUS_MANIFEST.json`.

Still **not** done, by design: no `git init`, no commit, no push, no remote
configured, no source script executed, no provider called, no model-research
catalog imported (D5 = defer). Course material is gated from any remote until
the Commander creates the **private** target and confirms visibility (D2);
see `docs/RELEASE_CHECKLIST.md` and the Phase 3 receipt in session records.
