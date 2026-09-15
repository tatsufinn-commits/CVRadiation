# `Brain/courses/` — study corpus (RADIATION v1.0.0)

This region holds the Commander's enrolled-course material. **The repository is
public during development by explicit Commander decision (2026-09-15).** Public
visibility is a custody choice, not a rights clearance: everything here is
retained for the Commander's **personal study**, is **not** represented as
public-domain or redistribution-permitted, and the Commander is responsible
for visibility and storage authorization. Rules are rewritten (M-013) from the
pinned v3 corpus policy; v3 validator machinery was not imported.

## Contract

1. **Every file here is an exact entry in `COURSE_CORPUS_MANIFEST.json`.** The
   manifest binds `path`, `sha256`, `media_type`, `role`, `load_policy`,
   privacy classification, source provenance (pinned blob SHA for imports),
   and the Commander approval reference. The check is bidirectional: no listed
   file may be missing and no file may be unlisted.
2. **Markdown derivatives are the normal AI-readable layer.** Source binaries
   (PDF/DOCX/HTML) are fidelity sources, loaded on demand when explicitly
   tasked; never re-hosted or redistributed.
3. **No redistribution claim.** Third-party school assets (syllabi,
   calendars, class schedules) are retained for the Commander's personal study
   under the Commander's authorization (D4, 2026-09-15; full-migration
   directive, 2026-09-15). A checksum is not a permission grant; nothing here
   marks redistribution rights, and public visibility does not create any.
4. **Personal data, accepted visibility.** Timetables and the calendar feed
   contain rooms, sections, and class times. The Commander has knowingly
   accepted their visibility in the public-during-development repository; the
   AI never republishes them elsewhere and cannot change repository
   visibility.
5. **On demand.** Load corpus derivatives when the study task needs them; do
   not treat them as truth about a subject — a syllabus says what is
   examinable, not what is true.
6. **No automated content inspection is claimed.** Manifests prove existence
   and digest, not semantic fidelity of a conversion; conversion limitations
   are recorded per asset.
7. **Additions** need a Commander order, a manifest entry, a hash check, and a
   `MIGRATION_LOG.md` row — in that order.

## What is deliberately absent

`desktop.ini`-style environment clutter; credential URLs or tokens; the v3
check tooling and JSON schema (deferred — M-036); broader collection materials
(external source lists, ingested reviewers, drills, session journals) excluded
from the v1 baseline under M-037…M-039, returnable only as individually
approved future items.
