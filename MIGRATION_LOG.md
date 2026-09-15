# MIGRATION LOG — RADIATION v1.0.0

Every imported or rewritten item is recorded with the six required fields:
**source path · source SHA (commit + blob; sha256 for binaries) · date · reason
· privacy classification · Commander approval reference** (plus action and
verification). Approval reference **CMD-2026-09-15-Dx** is the Commander's
in-session decision set of 2026-09-15 recorded in `MIGRATION_PLAN.md` §0.
Nothing is present in v1 without a row below. Source snapshot:
RADIATION@`fbce71bbfe4c62da71e6b347d36617474f840297`.

## A. Verbatim imports (Keep)

| # | v1 path | Action | Source path @ SHA | Date | Reason | Privacy | Verification | Approval |
|---|---|---|---|---|---|---|---|---|

| 1 | Brain/courses/AR153P.md | Keep (verbatim) | RADIATION@fbce71b `AR153P.md` blob `416073ffb051706e3761abbee8320196c9676496` | 2026-09-15 | AR153P Building Utilities 2 — enrolled-course digest | private — Commander study notes | blob SHA-1 == pinned (416073ffb0…); sha256 b895cd210b75db5d… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 2 | Brain/courses/AR163-1P.md | Keep (verbatim) | RADIATION@fbce71b `AR163-1P.md` blob `9333eb1f61333c2febda63cb44166af577e5f04a` | 2026-09-15 | AR163-1P Building Technology — enrolled-course digest | private — Commander study notes | blob SHA-1 == pinned (9333eb1f61…); sha256 df59c7840fd94da9… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 3 | Brain/courses/AR173-1P.md | Keep (verbatim) | RADIATION@fbce71b `AR173-1P.md` blob `ffb060ba3c28f0855defcf41de4c3390fc291d20` | 2026-09-15 | AR173-1P Urban Design & Community Architecture digest | private — Commander study notes | blob SHA-1 == pinned (ffb060ba3c…); sha256 43f87568a47a6c8c… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 4 | Brain/courses/CALENDAR.md | Keep (verbatim) | RADIATION@fbce71b `CALENDAR.md` blob `88bcfd544d831d5a64efeff5ec57611565fbe579` | 2026-09-15 | term calendar view for the assistant | private — Commander study notes | blob SHA-1 == pinned (88bcfd544d…); sha256 bc13c8e3dafbfa51… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 5 | Brain/courses/DSS10.md | Keep (verbatim) | RADIATION@fbce71b `DSS10.md` blob `cd770b2544a7e26816aa68666c9accb0f528b000` | 2026-09-15 | DSS10 Introduction to Data Science digest | private — Commander study notes | blob SHA-1 == pinned (cd770b2544…); sha256 fd20ac8fd8b95a56… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 6 | Brain/courses/GED103.md | Keep (verbatim) | RADIATION@fbce71b `GED103.md` blob `8dff0cb174be0d50b34654d9f20c1f072c2b192d` | 2026-09-15 | GED103 Readings in Philippine History digest | private — Commander study notes | blob SHA-1 == pinned (8dff0cb174…); sha256 e715c93e5f5c5550… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 7 | Brain/courses/MEC30-7.md | Keep (verbatim) | RADIATION@fbce71b `MEC30-7.md` blob `66a462014b83e32aac1722d051731952f92c7c87` | 2026-09-15 | MEC30-7 Statics of Rigid Bodies digest | private — Commander study notes | blob SHA-1 == pinned (66a462014b…); sha256 134edd8c971fdb29… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 8 | Brain/courses/SCHEDULE.md | Keep (verbatim) | RADIATION@fbce71b `SCHEDULE.md` blob `47d5848bbe3b22dec9b6b339a359be7056441446` | 2026-09-15 | human-readable weekly timetable (rooms/sections included by Commander decision) | private — personal timetable data | blob SHA-1 == pinned (47d5848bbe…); sha256 959bb294de869968… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 9 | Brain/courses/SCHEDULE.csv | Keep (verbatim) | RADIATION@fbce71b `SCHEDULE.csv` blob `9af9a3b8f19122a8dcb12ce348fce731867612b1` | 2026-09-15 | source timetable data | private — personal timetable data | blob SHA-1 == pinned (9af9a3b8f1…); sha256 3e1afa3672159f74… (matches old manifest) | CMD-2026-09-15-D4 |
| 10 | Brain/courses/0_CALLENDER/TERM1_FEED.txt | Keep (verbatim) | RADIATION@fbce71b `0_CALLENDER/TERM1_FEED.txt` blob `94cebd76cbfd5b16c7efef5aedd9761d5e225273` | 2026-09-15 | raw Blackboard calendar export for schedule upkeep | private — personal timetable data | blob SHA-1 == pinned (94cebd76cb…); sha256 9b3f614843cc4d12… (matches old manifest) | CMD-2026-09-15-D4 |
| 11 | Brain/courses/0_CALLENDER/readme.txt | Keep (verbatim) | RADIATION@fbce71b `0_CALLENDER/readme.txt` blob `cc5e019cc9ae1ab76595e303bd895849fe6649b6` | 2026-09-15 | one-line Commander note describing the feed | private — personal timetable data | blob SHA-1 == pinned (cc5e019cc9…); sha256 c3994dc1ef183eb8… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 12 | Brain/courses/AR173-1P_PLANNING_2/AR173-1P (Fundamentals of Urban Design and Community Architecture)-CLASS SCHEDULE.pdf | Keep (verbatim) | RADIATION@fbce71b `AR173-1P_PLANNING_2/AR173-1P (Fundamentals of Urban Design and Community Architecture)-CLASS SCHEDULE.pdf` blob `e9b231abb898a782da25f7b0e4945f2ea34ad221` | 2026-09-15 | MD derivative / course material | private — third-party school asset; Commander storage authorization D4; no redistribution | blob SHA-1 == pinned (e9b231abb8…); sha256 e10a43c2f37a9b80… (matches old manifest) | CMD-2026-09-15-D4 |
| 13 | Brain/courses/DSS10_INTRODUCTION_TO_DATA_SCIENCE/SOIT_DSS10_1Q_ Syllabus.docx | Keep (verbatim) | RADIATION@fbce71b `DSS10_INTRODUCTION_TO_DATA_SCIENCE/SOIT_DSS10_1Q_ Syllabus.docx` blob `29afdeb63a640e8742daa5d20dd04c4a462e6060` | 2026-09-15 | MD derivative / course material | private — third-party school asset; Commander storage authorization D4; no redistribution | blob SHA-1 == pinned (29afdeb63a…); sha256 99e388eccc2fc804… (matches old manifest) | CMD-2026-09-15-D4 |
| 14 | Brain/courses/DSS10_INTRODUCTION_TO_DATA_SCIENCE/SOIT_DSS10_1Q_Syllabus.md | Keep (verbatim) | RADIATION@fbce71b `DSS10_INTRODUCTION_TO_DATA_SCIENCE/SOIT_DSS10_1Q_Syllabus.md` blob `b898ec154a213993e83bf4b77044fd4512029dd0` | 2026-09-15 | MD derivative / course material | private — derivative of third-party school asset; same authorization | blob SHA-1 == pinned (b898ec154a…); sha256 dbfe7eeb9704a8be… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 15 | Brain/courses/GED103_READINGS_IN_PHILIPPINE_HISTORY/GED103 Syllabus_Q12627.docx | Keep (verbatim) | RADIATION@fbce71b `GED103_READINGS_IN_PHILIPPINE_HISTORY/GED103 Syllabus_Q12627.docx` blob `e334ab769da48bbb4c6c1682a10e3da7b827f825` | 2026-09-15 | MD derivative / course material | private — third-party school asset; Commander storage authorization D4; no redistribution | blob SHA-1 == pinned (e334ab769d…); sha256 eae44c07445e48f7… (DRIFT vs old manifest (declared eae44c07445f2a48f77aef95d4c78ee40652bca55c0c8141adcb92a061e4c5905a)) — v1 manifest records true digest; drift logged | CMD-2026-09-15-D4 |
| 16 | Brain/courses/GED103_READINGS_IN_PHILIPPINE_HISTORY/GED103_Syllabus_Q12627.md | Keep (verbatim) | RADIATION@fbce71b `GED103_READINGS_IN_PHILIPPINE_HISTORY/GED103_Syllabus_Q12627.md` blob `4493e5fc8010da0753786237a822c31c8b3586d4` | 2026-09-15 | MD derivative / course material | private — Commander study notes | blob SHA-1 == pinned (4493e5fc80…); sha256 e7f713c5fe5f2d19… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |
| 17 | Brain/courses/MEC30-7_STATICS_OF_RIGID_BODIES_FOR_CE/MEC30-7 Course Calendar 1Q.html | Keep (verbatim) | RADIATION@fbce71b `MEC30-7_STATICS_OF_RIGID_BODIES_FOR_CE/MEC30-7 Course Calendar 1Q.html` blob `66f837c087acfbd322c4a516f3589d6e97f38c60` | 2026-09-15 | MD derivative / course material | private — third-party school asset; Commander storage authorization D4; no redistribution | blob SHA-1 == pinned (66f837c087…); sha256 495da86995575418… (matches old manifest) | CMD-2026-09-15-D4 |
| 18 | Brain/courses/MEC30-7_STATICS_OF_RIGID_BODIES_FOR_CE/MEC30-7_Course_Calendar.md | Keep (verbatim) | RADIATION@fbce71b `MEC30-7_STATICS_OF_RIGID_BODIES_FOR_CE/MEC30-7_Course_Calendar.md` blob `87be883a25cf0949625868197ed26c0f805585db` | 2026-09-15 | MD derivative / course material | private — derivative of third-party school asset; same authorization | blob SHA-1 == pinned (87be883a25…); sha256 c21aea5aae4f5a85… (fresh sha256 (none declared before)) | CMD-2026-09-15-D4 |

## B. Rewrites and v1-handwritten files (no verbatim bytes imported)

| # | v1 path | Action | Source @ blob SHA | Date | Reason | Privacy | Verification | Approval |
|---|---|---|---|---|---|---|---|---|

| 19 | README.md | Rewrite | pinned `README.md` `3dff65a3…`, `PROTOCOL.md` `08fb5aa1` | 2026-09-15 | study-first v1 root statement | public-facing (v1 authorship) | visual review; no v3 version strings | CMD-2026-09-15-D3 |
| 20 | VERSION | New (exact) | none | 2026-09-15 | clean baseline marker | n/a | content exactly "v1.0.0" | CMD-2026-09-15-D3 |
| 21 | MIGRATION_SOURCES.md | New | inspection records 2026-09-15 | 2026-09-15 | provenance of sources/inspection | n/a | SHA/date review | CMD-2026-09-15-D3 |
| 22 | MIGRATION_PLAN.md | New | — (63 inventory rows, blob SHAs machine-checked vs live tree API) | 2026-09-15 | row-by-row migration plan | n/a | all cited blobs verified present in pinned tree | CMD-2026-09-15-D1..D6 |
| 23 | agents/INDEX.md | Rewrite | pinned `AGENTS.md` `dd38a5e9…`, `agents/AGENT_INDEX.md` `1b823f97…`, `agents/RESEARCH_METHOD.md` `aeeff712…` | 2026-09-15 | observed-host routing + research method | internal (public-source method) | visual review; five folders exist; no access claims | CMD-2026-09-15-D3 |
| 24 | agents/Arena_AI/README.md | New placeholder | pinned triad NOT imported (deferred per D3) | 2026-09-15 | honest placeholder | n/a | contains no capability/provider claim | CMD-2026-09-15-D3 |
| 25 | agents/ChatGPT/README.md | New placeholder | pinned triad NOT imported (deferred per D3) | 2026-09-15 | honest placeholder | n/a | same | CMD-2026-09-15-D3 |
| 26 | agents/Gemini/README.md | New placeholder | pinned triad NOT imported (deferred per D3) | 2026-09-15 | honest placeholder | n/a | same | CMD-2026-09-15-D3 |
| 27 | agents/Grok/README.md | New placeholder | pinned triad NOT imported (deferred per D3) | 2026-09-15 | honest placeholder | n/a | same | CMD-2026-09-15-D3 |
| 28 | agents/Claude/README.md | New placeholder | pinned triad NOT imported (deferred per D3) | 2026-09-15 | honest placeholder | n/a | same | CMD-2026-09-15-D3 |
| 29 | docs/.readme | Rewrite | pinned `docs/.readme` `9b86a0a9…`, `AGENTS.md` `dd38a5e9…`, `BOOT_SEQUENCE.md` `9dc8826a` | 2026-09-15 | short entry gate with no auto-discovery claim | public-facing (v1 authorship) | visual review; referenced paths exist; no mode/tier machinery | CMD-2026-09-15-D3 |
| 30 | docs/PROJECT_SCOPE.md | Rewrite | pinned `README.md` `3dff65a3…`, `PROTOCOL.md` `08fb5aa1` | 2026-09-15 | study-first scope + stop-lines | public-facing (v1 authorship) | visual review vs scope order §1 | CMD-2026-09-15-D3 |
| 31 | docs/PASS_HANDOFF.md | Rewrite (concept) | pinned `agents/_common/radiation_pass.py` `6a870eb2…` READ AS TEXT, never executed; `BOOT_SEQUENCE.md` `9dc8826a` | 2026-09-15 | bounded zero-write handoff card with all order §7.2 fields | n/a | field checklist; verbatim non-elevation sentence present; no .py copied | CMD-2026-09-15-D3 |
| 32 | docs/RELEASE_CHECKLIST.md | Rewrite (lesson) | pinned `VERSIONING_GUIDE.md` `7ebed87c…`, `docs/PATCH_PROTOCOL.md` `75ec75bc…` | 2026-09-15 | seven-item release checklist (order §7.3) | n/a | item-by-item match to order §7.3 | CMD-2026-09-15-D3 |
| 33 | Brain/courses/README.md | Rewrite | pinned `docs/COURSE_CORPUS_POLICY.md` `6c9f4c4b…` | 2026-09-15 | private corpus contract | private | visual review; wording states PRIVATE | CMD-2026-09-15-D3/D4 |
| 34 | Brain/courses/INDEX.md | Rewrite | pinned `Brain/courses/INDEX.md` `ddc603ce…` | 2026-09-15 | clean six-course register; v3 patch refs removed | private | visual review; schedule figures cross-check SCHEDULE.csv | CMD-2026-09-15-D4 |
| 35 | Brain/courses/COURSE_CORPUS_MANIFEST.json | Rewrite (rebaseline) | pinned `Brain/courses/COURSE_CORPUS_MANIFEST.json` `ea89ffcc…` | 2026-09-15 | v1 source/hash/permission declaration | private | JSON parses; bidirectional file↔manifest check; sha256 recomputed | CMD-2026-09-15-D4 |

## C. Findings recorded at import

1. **Digest drift (GED103 DOCX):** the pinned v3 manifest declares
   `sha256:eae44c07…c5905a` for `GED103 Syllabus_Q12627.docx`; the file actually
   present in the pinned git tree (verified by git blob SHA-1 equality, and a
   valid OOXML zip) has a different sha256, recorded in the v1 manifest. The old
   declaration was wrong; nothing in v1 copies it. All other declared binaries
   matched (PDF, DSS10 DOCX, MEC HTML, CSV, feed).
2. **Secret scan:** `0_CALLENDER/TERM1_FEED.txt` contains no credential URL
   (only the public tzurl.org timezone reference). Open Commander item P4
   (rotation of the feed URL historically committed in old commit `4a98e59`)
   is unrelated to the file content and stays open until the Commander closes it.
3. **Privacy gate:** files exist only in the local workspace. None may be
   pushed until the Commander creates the private RADIATION-v1 and confirms
   visibility (D2); the release checklist enforces this.

## D. Excluded without import (recorded in MIGRATION_PLAN.md)

M-011, M-034, M-036 (deferred), M-037…M-039 (baseline exclusions / future
per-item), M-040…M-055 (deferred past v1.0.0 by D5), M-056…M-063 (v3 machinery,
evidence, scaffolding, modes/cue/styles/subskills, bulk docs, schemas, history;
excluded by D6), and every §2.3 carrier family (zero found at the pinned
snapshot; fail-closed scan repeated in the release checklist).
