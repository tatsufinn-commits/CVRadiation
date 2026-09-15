# MIGRATION SOURCES

What this migration may look at, what it may not use, and how inspection was
performed.

## 1. Target repository (this repository)

| Field | Value |
|---|---|
| Target | https://github.com/tatsufinn-commits/CVRadiation.git |
| Visibility | **Public during development — explicit Commander decision, full public migration directive 2026-09-15** |
| Public HEAD reviewed in the directive | `8d2dba8cc3f3e2bb677c6253b2dec5c7ca308714` ("Add v1 study corpus and migration docs") |
| Phase A refresh | Local read-only clone confirmed HEAD = `8d2dba8…`; 116 tracked files |
| Push authority | Commander only; the AI prepares Phase A locally and stops for the phrase `Approve full v1 archive migration` before any commit/push |

The earlier D1 plan (fresh private `RADIATION-v1`) is **superseded** by the
Commander's full-public-migration directive of 2026-09-15. The directive keeps
all other governance: plan-first gating, no source execution, no AI push,
no carrier artifacts, dated-or-unverified claims.

## 2. Source snapshot (the ONLY old-repo content used)

| Field | Value |
|---|---|
| Old repository | https://github.com/tatsufinn-commits/RADIATION.git |
| Source commit | `fbce71bbfe4c62da71e6b347d36617474f840297` |
| Source tree SHA | `c8d85e7c19bd10500efc2d400b08c26b379a51f6` |
| Commit date | 2026-09-15T02:39:29Z |
| Snapshot size | 176 directories, **835 tracked blobs** (verified by `git ls-files` at the pinned checkout and the GitHub tree API) |
| Role in v1 | **Inert historical archive only** — copied byte-for-byte to `legacy/RADIATION_v3_fbce71b/`; see `docs/LEGACY_BOUNDARY.md` |

## 3. Excluded by instruction

| Reference | Status |
|---|---|
| Current old `main` `e206375783f13216ea9e73b78549517e21d42c09` and later carrier commits `d7d1695`, `62a5574`, `98d8c81`, `0a58a9c` | **Not a source**; not checked out or copied; only named per the directive |
| v3 delivery reports, local candidates, ZIPs, named branches, prose reports | Not proof of public state; not used |
| Forbidden carriers (`APPLY.sh/.ps1`, `*.zip`, `RADIATION_PATCH_*`, `PATCH.diff`, `append-block(s)/`, `*_STAGED*`, `*_DIFF*`, `*_REPLACEMENT*`, delivery reports) | Not imported into the active layer; historical copies exist only inside the inert archive, never executed |
| Unaccepted 5824 Release Truth Gate; P-11 / "55%" cue-audit claims | Not imported; release lesson rewritten small as `docs/RELEASE_CHECKLIST.md` |

## 4. How inspection and copying were done

- Read-only GitHub API/raw inspection (2026-09-15) and, for the full archive,
  a local `git clone` of the old repository with a **detached checkout of
  `fbce71b` only**; the red `main` was never checked out.
- Archive bytes were exported with `git archive fbce71b … | tar -x` into
  `legacy/RADIATION_v3_fbce71b/` — an exact tracked-tree copy that executes
  nothing. Exactly two Git-control filenames were neutralized per directive
  §2 (`.gitignore` → `DOT_gitignore.archived`, `.gitattributes` →
  `DOT_gitattributes.archived`); contents are byte-identical and mapped in
  `MIGRATION_ARCHIVE_MANIFEST.json`.
- Every archived file was verified against its source git blob SHA-1
  (`"blob <size>\0" + content`) and recorded with its target sha256: 835/835
  exact, no omissions, no unlisted archive files, exactly two renames.
- No source script, workflow, test, or relay was run in any phase; archived
  workflows remain nested (they cannot run in GitHub Actions) and no root
  `.github/` exists.
- The 18 active corpus files were byte-verified against pinned blobs during
  the original migration build; the same 18 shared files exist in the archive.

## 5. Visibility truth (per directive §5)

The initial Group D course corpus entered public CVRadiation in commit
`8d2dba8` on 2026-09-15 **while the target was public**, before an explicit
public-corpus decision was recorded in the directive. The directive now makes
public development the Commander's explicit, informed decision. This log does
not claim historical public exposure was impossible or harmless; public
history may persist in caches/forks, and the Commander owns the visibility and
storage-authorization judgment. Material labels remain "personal study / no
redistribution." The AI cannot change visibility or publish.
