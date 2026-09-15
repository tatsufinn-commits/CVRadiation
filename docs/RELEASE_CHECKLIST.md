# RELEASE CHECKLIST — RADIATION v1.0.0

The only release process v1 has. Every item is signed off by the Commander;
the AI prepares evidence but never pushes. Rewritten as a lesson from the v3
release history; the unaccepted 5824 "Release Truth Gate" machinery itself was
not imported (M-014).

## 1. Exact intended file list

- [ ] The tree contains exactly the files listed for the approved M-IDs in
      `MIGRATION_PLAN.md` — no more, no less.
- [ ] `VERSION` contains exactly `v1.0.0`; no file claims v3.x versioning.
- [ ] A complete file list is attached to the release request.

## 2. Source and approval entries

- [ ] Every imported or rewritten item has a `MIGRATION_LOG.md` row: source
      path, source SHA (pinned commit + blob SHA; sha256 for binaries), date,
      reason, privacy classification, Commander approval reference.
- [ ] Rewritten files were visually checked against their named source blobs;
      copied files match their blob SHA / declared hashes.

## 3. Visibility and study-materials check (public during development)

- [ ] The Commander has **explicitly reconfirmed**, at each corpus push, that
      CVRadiation is public during development and accepts that the listed
      course files (incl. PDF/DOCX/HTML and personal timetable/feed) become
      part of public history; the AI cannot change visibility or publish.
- [ ] `COURSE_CORPUS_MANIFEST.json` lists every file under `Brain/courses/`
      with matching sha256, and nothing exists there unlisted; every entry
      carries personal-study / no-redistribution labels.
- [ ] Third-party school assets carry the Commander's storage authorization
      (D4, 2026-09-15; full-migration directive, 2026-09-15); nothing is
      marked redistribution-permitted, and public visibility is recorded as a
      Commander responsibility, not a rights clearance.
- [ ] No credentials, tokens, or secret URLs: the calendar feed has been
      scanned; the LMS feed-credential rotation (P4) status is stated
      truthfully at push time (removing a URL does not revoke it).
- [ ] The Commander acknowledges public history is not reliably erased
      (caches/forks) — visibility decisions are taken before push, not after.

## 4. No forbidden carrier or patch files

- [ ] Fail-closed scan finds none of: `APPLY.sh`, `APPLY.ps1`, `*.zip`,
      `RADIATION_PATCH_*`, `PATCH.diff`, `*_DIFF*`, `append-blocks/`,
      `append_blocks/`, `*_STAGED*`, `*_REPLACEMENT*`, delivery reports, the
      5824 Release Truth Gate, or P-11/55%-claim artifacts **in the active
      layer** (historical copies may exist only inside the inert
      `legacy/RADIATION_v3_fbce71b/` archive).
- [ ] No active v3 executable machinery: no root `scripts/`,
      `radiation_core/`, root `.github/workflows/`, or relays; archived
      copies under `legacy/` are nested, unwired, and never executed.
- [ ] `MIGRATION_ARCHIVE_MANIFEST.json` has exactly 835 entries, every
      archive file matches its pinned blob SHA-1, exactly the two approved
      Git-control renames exist, and no unlisted archive file is present.

## 5. Commander diff review

- [ ] The AI presents the complete changed-file list and the full diff.
- [ ] The Commander explicitly states the build is ready. Praise, silence, or
      a prior session does not count as approval.

## 6. Push discipline

- [ ] The AI does not commit or push. No collaborator invites, deployments, or
      provider calls occur.
- [ ] The Commander performs the commit and the v1.0.0 push after approval.

## 7. Post-push verification

- [ ] On a fresh clone of the actual remote, the remote HEAD SHA contains
      exactly the intended files with matching hashes (the manifest verifies
      from the clone, not from the build workspace).
- [ ] Only then is v1.0.0 recorded as released.
