# Courses — the Commander's enrolled-term register (RADIATION v1.0.0)

The join key between the study assistant and the timetable. Rewritten for v1
(M-016) from the pinned `Brain/courses/INDEX.md`; v3 patch history, external
registry IDs, and references to collections not carried into v1 were removed.

## Term 1, AY 2026–2027 — six courses, 18 units

| Code | Title | Units | v1 materials |
|---|---|:--:|---|
| GED103 | Readings in Philippine History | 3 | digest + syllabus (DOCX + MD derivative) |
| DSS10 | Introduction to Data Science (with Coursera) | 3 | digest + syllabus (DOCX + MD derivative); Coursera is external |
| MEC30-7 | Statics of Rigid Bodies for CE | 3 | digest + course calendar (HTML + MD derivative) |
| AR173-1P | Planning 2 — Urban Design & Community Architecture | 3 | digest + class schedule PDF |
| AR163-1P | Building Technology | 3 | digest only (see "not carried into v1") |
| AR153P | Building Utilities 2 | 3 | digest only (see "not carried into v1") |

## Weekly meeting pattern

- **36.0 contact-hours per week over five days** — Mon 9.0 · Tue 6.0 · Thu 3.0
  · Fri 7.5 · Sat 10.5. **Wednesday and Sunday are clear.**
- 07:30 starts on Mon, Tue, Thu, Sat.
- Authoritative timetable: `SCHEDULE.md` / `SCHEDULE.csv` (rooms and sections
  included by the Commander's explicit decision; the repository is public
  during development by Commander decision and the material is personal-study,
  not redistribution-permitted). When a class relocates,
  update those files — a stale room is worse than no room.
- `CALENDAR.md` is the term calendar view; `0_CALLENDER/TERM1_FEED.txt` is the
  raw Blackboard export it can be refreshed from (data, not a credential).

## Materials rules

- Syllabi and calendars say what is **examinable**, not what is true.
- Every file in this folder is manifest-declared (`COURSE_CORPUS_MANIFEST.json`)
  with hash, role, and permission status; source binaries load on demand.
- A syllabus digest without its source binary still records what the syllabus
  said; a missing syllabus delays planning, not study support.

## Not carried into v1.0.0 (possible future, each needs its own approval)

- The large ingested reviewer collections for AR163-1P / AR153P (building
  technology and utilities books/reviewers), image-only pages, and external
  source lists — excluded at the baseline (M-037/M-039), not deleted from
  history; they can return as individually approved corpus items.
- Drill sets, Anki TSVs, nota cards, and planning-reviewer audits from the v3
  work folders — same status (M-039).
