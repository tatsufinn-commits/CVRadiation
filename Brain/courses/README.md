# `Brain/courses/` — private study corpus (RADIATION v1.0.0)

This region holds the Commander's enrolled-course material in a **private**
repository. Rules rewritten (M-013) from the pinned v3 corpus policy; v3
validator machinery was not imported.

## Contract

1. **Every file here is an exact entry in `COURSE_CORPUS_MANIFEST.json`.** The
   manifest binds `path`, `sha256`, `media_type`, `role`, `load_policy`,
   privacy classification, source provenance (pinned blob SHA for imports),
   and the Commander approval reference. The check is bidirectional: no listed
   file may be missing and no file may be unlisted.
2. **Markdown derivatives are the normal AI-readable layer.** Source binaries
   (PDF/DOCX/HTML) are fidelity sources, loaded on demand when explicitly
   tasked; never re-hosted or redistributed.
3. **Private only.** Third-party school assets (syllabi, calendars, class
   schedules) are retained for the Commander's personal study under the
   Commander's authorization (decision D4, 2026-09-15). A checksum is not a
   permission grant; nothing here marks redistribution rights.
4. **Personal data.** Timetables and the calendar feed contain rooms,
   sections, and class times. They live only in the private repository.
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
