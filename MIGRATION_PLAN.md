# MIGRATION PLAN — RADIATION v1.0.0

**Plan date:** 2026-09-15 (Asia/Singapore)  
**Planner:** new AI (migration analyst; not an autonomous publisher)  
**Status:** APPROVED FOR PHASE 2 BUILD (Commander, in-session decisions 2026-09-15). See §0.

## 0. Approval record (2026-09-15, Asia/Singapore)

| Decision | Commander ruling | Effect |
|---|---|---|
| D1 — target | Fresh **private** RADIATION-v1 to be created by the Commander; AI builds the tree locally in the workspace; no remote action by the AI | remote/push gated on Commander |
| D2 — privacy gate | Corpus may be built into the LOCAL tree; nothing course-related reaches any remote until the Commander confirms the new repository is private | gate stands before push |
| D3 — framework M-001…M-015 | APPROVED; provider profiles M-005…M-009 ship as honest **placeholders** (dated profile content not imported) | placeholders built |
| D4 — corpus M-016…M-036 | APPROVED all 21 course files including the four school binaries + three MD derivatives; Commander attests private-study authorization; M-034 desktop.ini excluded; M-035 manifest rebaselined; M-036 deferred | imported locally with hashes/log rows |
| D5 — model research M-040…M-056 | DEFERRED past v1.0.0 | nothing built |
| D6 — bulk exclusions M-057…M-063 + §5 | No contrary instruction; excluded per plan | enforced by scans |

Approval reference used in `MIGRATION_LOG.md`: **CMD-2026-09-15-D1..D6**.

---
**Only inspected source:** `https://github.com/tatsufinn-commits/RADIATION.git`
@ commit `fbce71bbfe4c62da71e6b347d36617474f840297`
(tree `c8d85e7c19bd10500efc2d400b08c26b379a51f6`, 2026-09-15T02:39:29Z,
835 files / 176 directories). Full provenance in `MIGRATION_SOURCES.md`.

---

## 1. Plain-language summary for the Commander

**What I recommend KEEPING (after you approve, and only into a private target):**

- Your study records under `Brain/courses/`: the six course digests, the term
  calendar, the schedule MD/CSV, and the three Markdown syllabus/calendar
  derivatives — these ARE the study assistant.
- The calendar feed export and its one-line note (I secret-scanned the feed:
  it contains **no** credential URL — only a public timezone reference).
- The four original source assets (1 PDF class schedule, 2 DOCX syllabi, 1 HTML
  calendar) **only if you confirm** you are authorized to store them; they live
  in a private repository and never get republished.
- **Optionally**, the 14 model-research JSON records with their source register
  and 16 receipts — as a clearly-labelled, not-yet-revalidated research snapshot.
  Never as a routing/deployment rule. My recommendation is to defer this layer.

**What I recommend REWRITING (small, v1-flavored, no v3 history carried over):**

- The root README and a short `docs/PROJECT_SCOPE.md` from the mission language
  in the old README/PROTOCOL — study-first, dropping the "operating system" sprawl.
- A tiny `docs/.readme` entry gate that tells a runtime *which is already able
  to read the repository* to open its named `agents/<Provider>/` folder — with no
  claim that any product auto-discovers or browses folders.
- The provider index and five provider READMEs from the old `agents/` BOOT /
  CAPABILITY_PROFILE / SOURCES files — keeping dated claims, source lists, and
  the "model identity unknowable / tools session-contingent" red lines, dropping
  references to the v3 control plane, probes, and pass script.
- The RADIATION PASS idea as a short **markdown handoff card**
  (`docs/PASS_HANDOFF.md`), explicitly zero-write and non-elevating; the old
  14 KB Python state machine is **not** imported or run.
- The release-discipline lesson as a one-page `docs/RELEASE_CHECKLIST.md`.
- The course manifest, rebaselined for v1, empty until per-item approvals land.

**What I recommend EXCLUDING:**

- Everything that makes v3 heavy and red: `radiation_core/`, `scripts/`,
  `tools/`, CI workflows, `tests/`, `evals/`, `evidence/` (383 receipt files),
  `outputs/`, `scaffolding/` (112), `styles/`, `subskills/`, `cue/`, the 42
  phase work-product folders, 39 bulk `docs/` files (AI_RULES, CAPABILITIES,
  KNOWLEDGE_REGISTRY, OPEN_SOURCES, PATCH_LEDGER, ROADMAP, shrine, …), 13
  orphaned schemas, and the 74 KB CHANGELOG. v1 history starts at v1.0.0.
- The routing matrix (self-labelled "unmeasured impressions"), eval-harness and
  deployment-matrix design docs, and all provider-call/credential/deployment
  machinery (order §6.3).
- **All forbidden carrier families** — see §5; a filename scan of the pinned
  snapshot found **zero** of them, and the v1 checklist fails the build if any appear.
- `desktop.ini` (OS clutter).

**Items needing a privacy or copyright answer from you (§6):**

1. The target repository must be **confirmed private before any corpus file
   moves**. The `CVRadiation` repository you linked is currently **public**.
2. The four school assets (PDF/DOCX/DOCX/HTML) and their three Markdown
   derivatives derive from university-produced material — your authorization
   call; checksums are not permission.
3. Schedule/feed files carry your personal timetable (rooms, sections, class
   times). You permitted this in the *old public* repo (amendment A1); v1 is a
   fresh, private-repo decision.
4. A credentialed calendar URL was committed to old history on 2026-09-13 and
   its source-side rotation was still marked pending — that item is yours to
   close; the feed file itself does not contain the URL.
5. `Brain/external_sources/` (book/reviewer link lists) and study drills / nota
   cards in `01…09/` are future per-item corpus candidates, not v1.0.0.

**Runtime/provider capabilities that remain UNVERIFIED (§7):**

1. Whether ChatGPT, Gemini, Grok, or Claude hosted sessions can browse and
   select repository folders from a paste / magic-words handoff — never
   observed; the v1 `.readme` will not claim it.
2. This Arena session's tools are observed **for this session only** (file
   workspace, shell, web fetch/search; no push credentials seen) and are not
   generalized to the platform.
3. Provider profiles are dated 2026-09-14/15 with a 90-day review trigger
   (2026-12-13) and are **not re-verified for v1**. Observed status change
   2026-09-15: `arena.ai/privacy`, `/terms`, `/pricing` now answer HTTP 200
   (404/reCAPTCHA in the dated research); contents unreviewed — a live review
   trigger, not a claim.
4. The 14 model records are a 2026-09-15 sweep; some retention/training strings
   rest on secondary or reserved-domain `.example` sources the records
   themselves flag as weak. Revalidate before any policy claim.

---

## 2. Actions and rules used in this plan

- **Keep** = copy content into v1 (corpus only after the private-repo gate and
  item approval; hash-verified).
- **Rewrite** = handwrite a small v1 document using the source as reference; no
  wholesale lifting; v3 patch numbers, ledger refs, and machinery names removed.
- **Exclude** = do not import; listed so the decision is explicit and reviewable.
- Every SHA below is the **40-character git blob SHA at the pinned commit** (the
  immutable content address). The plan's SHAs were machine-checked against the
  live GitHub tree API on 2026-09-15 (all 835 blobs match the inspection cache).
  Binaries additionally carry the SHA-256 declared in the old corpus manifest.
- Rewrite rows import **no bytes**; at Phase 3 rewritten files are verified by
  visual review against the named source blobs, not by hash equality.

---

## 3. Intended v1 tree after an approved Phase 2

```text
RADIATION-v1/
├── README.md                 # handwritten (informed by M-001)
├── VERSION                   # exactly: v1.0.0
├── MIGRATION_SOURCES.md      # handwritten (present)
├── MIGRATION_PLAN.md         # this file (present)
├── MIGRATION_LOG.md          # import ledger (present; empty)
├── agents/
│   ├── INDEX.md              # rewritten from M-002/M-004/M-010
│   ├── ChatGPT/README.md     # placeholder or dated profile (M-006)
│   ├── Gemini/README.md      # placeholder or dated profile (M-007)
│   ├── Grok/README.md        # placeholder or dated profile (M-008)
│   ├── Claude/README.md      # placeholder or dated profile (M-009)
│   └── Arena_AI/README.md    # placeholder or dated profile (M-005)
├── docs/
│   ├── .readme               # rewritten v1 entry gate (M-002/M-003/M-015)
│   ├── PROJECT_SCOPE.md      # handwritten, informed by M-001
│   ├── PASS_HANDOFF.md       # handwritten card; concept from M-012/M-015
│   └── RELEASE_CHECKLIST.md  # handwritten; lesson from M-014
└── Brain/
    └── courses/
        ├── COURSE_CORPUS_MANIFEST.json   # rebaselined (M-035); EMPTY until approvals
        ├── README.md                     # optional short corpus rules (M-013)
        └── …approved corpus items only (M-016…M-033)
```

Provider READMEs are **placeholders** unless the corresponding M-ID is approved
together with its dated sources; "placeholder" is honest — invented capability
claims are not.

---

## 4. Row-by-row import inventory

### Group A — Purpose and task boundary
| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-001 | `README.md` @ `3dff65a345b8e88ca764d4e6a00ccccb136a421a`; `PROTOCOL.md` @ `08fb5aa1ce84b6a228a0e1dd71b73e5ab9969a92` | `README.md` (root); `docs/PROJECT_SCOPE.md` | Rewrite | Concise study-first mission, name, and authority statements; drops the six-mode/OS sprawl and v3 lineage claims | public-facing prose; rewrite = v1 authorship | visual diff vs the two source blobs; no v3 version strings (`v3.10.x`, "58xx" patches) remain; Commander review | APPROVED (D3) |
| M-002 | `AGENTS.md` @ `dd38a5e91ec23f5f508f61913514d537e91fff92` | concepts → `docs/.readme`, `agents/INDEX.md` | Rewrite | Its honesty clause ("repository text cannot force a product to load it") and observed-host routing rule are the core of the v1 provider index | public-facing prose | visual review; confirm no claim of auto-discovery, tools, or authority | APPROVED (D3) |
| M-003 | `docs/.readme` @ `9b86a0a9a81c894c5daa37f80445e0b0a5bae807` | `docs/.readme` | Rewrite | v1 entry gate: directs a runtime that can already read the repo to its named provider folder; states limits | public-facing prose | visual review; link test of every referenced v1 path; no tier/mode machinery | APPROVED (D3) |

### Group B — Provider-facing index (`agents/`)
| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-004 | `agents/AGENT_INDEX.md` @ `1b823f97ee57344208c07db9e1c0063604b0b751` | agents/INDEX.md | Rewrite | Exact five-folder routing table; observed-host-only rule; unknown→generic fallback; "convention, not proof" limitation | internal research notes from public sources | visual review; exact five folder names exist; no routing automation referenced | APPROVED (D3) |
| M-005 | `agents/Arena_AI/BOOT.md` @ `7ee8f1a6e5626b2507d1d31a7e7dedbf37a8b10c`; `agents/Arena_AI/CAPABILITY_PROFILE.md` @ `c6907384f63e4fcc006d09b8aa188c64fb8d79b8`; `agents/Arena_AI/SOURCES.md` @ `13e43c5b75253349b5ce6c7aea0ca5c9a8fc539e` | agents/Arena_AI/README.md | Rewrite | Profile for THIS session host; keeps dated sources (arena.ai/agent 2026-09-14; chatgate/stork 2026-06-05), the unknowable-model red line, and privacy/pricing gaps; drops probe/control-plane references | internal research; public-source citations | every retained claim traced to a dated source row; today's 200-vs-404 page-status change recorded; no model name asserted | APPROVED — placeholder README only (D3) |
| M-006 | `agents/ChatGPT/BOOT.md` @ `a4641287fb8aa39c5eb299f60f25b2c391c4accc`; `agents/ChatGPT/CAPABILITY_PROFILE.md` @ `dc0b17c51dabbb03782b2dff37765cb1cf4f2bf8`; `agents/ChatGPT/SOURCES.md` @ `3f52922d364b3de35e50b35849b2da7e1861078a` | agents/ChatGPT/README.md | Rewrite | Dated provider profile; session-contingent posture | internal research; public-source citations | claim-to-source trace; folder-browse capability explicitly NOT claimed | APPROVED — placeholder README only (D3) |
| M-007 | `agents/Gemini/BOOT.md` @ `c6c8f4bb0ab6e126011b4c1b3003983c370f0946`; `agents/Gemini/CAPABILITY_PROFILE.md` @ `4f0717a987a71ff98c6c178a9317b38dd6564216`; `agents/Gemini/SOURCES.md` @ `6b911fa0a610508741a8f7139d95d128e23d669d` | agents/Gemini/README.md | Rewrite | Dated provider profile; session-contingent posture | internal research; public-source citations | same as M-006 | APPROVED — placeholder README only (D3) |
| M-008 | `agents/Grok/BOOT.md` @ `c78b3c8d93b6a3da44a1cb936d8a24c6fe1dc4a9`; `agents/Grok/CAPABILITY_PROFILE.md` @ `e3ebaccd75f64433362ac890b3cca1d0258df3ec`; `agents/Grok/SOURCES.md` @ `197226b6586aab79181a667d21fb588644f3e5ad` | agents/Grok/README.md | Rewrite | Dated provider profile; session-contingent posture | internal research; public-source citations | same as M-006 | APPROVED — placeholder README only (D3) |
| M-009 | `agents/Claude/BOOT.md` @ `f558d025bf73bf6dc5c5e2b2f7dbde5ee3be0e6e`; `agents/Claude/CAPABILITY_PROFILE.md` @ `4ddfe07cd804e4ed4f410f89877f8b0a0886a775`; `agents/Claude/SOURCES.md` @ `205e2f328095eceb98b4dc7fe352d4d5e4c6db8e` | agents/Claude/README.md | Rewrite | Dated provider profile; session-contingent posture | internal research; public-source citations | same as M-006 | APPROVED — placeholder README only (D3) |
| M-010 | `agents/RESEARCH_METHOD.md` @ `aeeff7126671fcd671a55039a74fc35139092255` | method appendix inside agents/INDEX.md | Rewrite | Evidence tiers [O]/[S]/[U]/[B], conflict/gap discipline, 90-day review trigger — the honesty method for maintaining profiles | internal method prose | visual review; review dates preserved on every volatile claim | APPROVED (D3) |
| M-011 | `agents/ROUTING_MATRIX.md` @ `d513ca11d9c47e972a8c65cb6dbfb1555e75ad49` | — | Exclude | Self-declared "unmeasured impressions"; v1 makes no model routing decisions (order §6.3); rebuildable only after a named local evaluation | — | post-build grep confirms no ratings matrix exists in v1 | EXCLUDED (D3/D6) |
| M-012 | `agents/_common/radiation_pass.py` @ `6a870eb2b98b0dbcfcdb88e68912751dde1dbffe` | code excluded; concept → docs/PASS_HANDOFF.md | Exclude + Rewrite concept | The five-yield handoff concept (routing, observed tools, boundary, profile, proofs) is wanted; the 14 KB script imports v3 probe/relay machinery, was never executed by this migration, and has no place in study-first v1 | code (read as data; unexecuted) | handoff card contains all order §7.2 fields plus the verbatim non-elevation sentence; grep confirms the .py is not copied | APPROVED (D3) |

### Group C — Governance and release discipline
| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-013 | `docs/COURSE_CORPUS_POLICY.md` @ `6c9f4c4b8070c54b5a5a7f4d04a4816b9c6853c8` | optional Brain/courses/README.md (short) | Rewrite | Corpus contract: manifest declares every non-text asset; checksum ≠ permission; on-demand loading; no content scanning claimed | internal governance prose | visual review; v1 wording must say PRIVATE (the old text says the old repo is public — that sentence is dropped/reversed) | APPROVED (D3) |
| M-014 | `VERSIONING_GUIDE.md` @ `7ebed87cda41dc86092355df3a80be675e3e55e1`; `docs/PATCH_PROTOCOL.md` @ `75ec75bc8011e66fdd4fca5defee2e54747d4319` | docs/RELEASE_CHECKLIST.md | Rewrite (lesson only) | The usable lesson from failed releases: file list, provenance entries, privacy check, no carrier files, Commander diff review, Commander-only push, post-push remote-SHA check | internal prose | checklist matches order §7.3's seven items exactly; no patch-zip workflow survives | APPROVED (D3) |
| M-015 | `BOOT_SEQUENCE.md` @ `9dc8826a73a5abd77ab8802f3ce4f2a3b86f97ef` | concepts → docs/.readme + docs/PASS_HANDOFF.md | Rewrite concept / Exclude file | The "declare what you loaded; degrade honestly" idea is useful; the v3 tier graph (task ledger, AI_RULES, passives) does not exist in v1 | internal prose | visual review; no references to files v1 will not contain | APPROVED (D3) |

### Group D — Study corpus (`Brain/courses/`, 21 files at the snapshot) — PRIVATE REPO GATE

> **Gate (order §1, §4):** none of M-016…M-033 is copied until the Commander
> confirms the target is **private**. The rebaselined manifest M-035 is created
> empty first; each approved item is then logged in `MIGRATION_LOG.md` with source
> path, source blob SHA, date, reason, privacy class, and approval reference.

| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-016 | `Brain/courses/INDEX.md` @ `ddc603ceea9ee922018758c9b5f17001391a949d` | Brain/courses/INDEX.md | Rewrite | Six-course register and weekly load pattern — the study join-key | private; Commander-authored, contains personal schedule framing | visual review; strip v3 patch refs (2600/5100/5500); schedule facts cross-checked to M-024/M-025 | APPROVED — Rewrite (D4) |
| M-017 | `Brain/courses/AR153P.md` @ `416073ffb051706e3761abbee8320196c9676496` | same | Keep | Building Utilities 2 digest — enrolled course | private study notes | blob-SHA equality at copy; visual scan for stray personal identifiers | APPROVED — Keep (D4; private gate before remote) |
| M-018 | `Brain/courses/AR163-1P.md` @ `9333eb1f61333c2febda63cb44166af577e5f04a` | same | Keep | Building Technology digest — enrolled course | private study notes | blob-SHA equality; same visual scan | APPROVED — Keep (D4; private gate before remote) |
| M-019 | `Brain/courses/AR173-1P.md` @ `ffb060ba3c28f0855defcf41de4c3390fc291d20` | same | Keep | Urban Design & Community Architecture digest (highest exam yield) | private study notes | blob-SHA equality; same visual scan | APPROVED — Keep (D4; private gate before remote) |
| M-020 | `Brain/courses/CALENDAR.md` @ `88bcfd544d831d5a64efeff5ec57611565fbe579` | same | Keep | Term calendar view for the assistant | private; derived data | blob-SHA equality; check Generated date; mark stale-as-of if not regenerated | APPROVED — Keep (D4; private gate before remote) |
| M-021 | `Brain/courses/DSS10.md` @ `cd770b2544a7e26816aa68666c9accb0f528b000` | same | Keep | Introduction to Data Science digest | private study notes | blob-SHA equality; visual scan | APPROVED — Keep (D4; private gate before remote) |
| M-022 | `Brain/courses/GED103.md` @ `8dff0cb174be0d50b34654d9f20c1f072c2b192d` | same | Keep | Readings in Philippine History digest | private study notes | blob-SHA equality; old edit redacted URLs to plain domains — confirm no scheme reintroduced | APPROVED — Keep (D4; private gate before remote) |
| M-023 | `Brain/courses/MEC30-7.md` @ `66a462014b83e32aac1722d051731952f92c7c87` | same | Keep | Statics of Rigid Bodies digest | private study notes | blob-SHA equality; visual scan | APPROVED — Keep (D4; private gate before remote) |
| M-024 | `Brain/courses/SCHEDULE.md` @ `47d5848bbe3b22dec9b6b339a359be7056441446` | same | Keep | Human-readable weekly timetable; the scheduling core | private; rooms/sections by your prior explicit decision | blob-SHA equality; table cross-checked against M-025 | APPROVED — Keep (D4; private gate before remote) |
| M-025 | `Brain/courses/SCHEDULE.csv` @ `9af9a3b8f19122a8dcb12ce348fce731867612b1` | same | Keep | Source timetable data; future re-derivation | private personal data; private-repo only | sha256 equality `3e1afa3672159f744f8f5a52c4f0d32fb1f0927bcc602d7b4d370122a5107618`; CSV parse check; private gate | APPROVED — Keep (D4; private gate before remote) |
| M-026 | `Brain/courses/0_CALLENDER/TERM1_FEED.txt` @ `94cebd76cbfd5b16c7efef5aedd9761d5e225273`; `Brain/courses/0_CALLENDER/readme.txt` @ `cc5e019cc9ae1ab76595e303bd895849fe6649b6` | same paths | Keep | Raw Blackboard calendar export for schedule upkeep; one-line Commander note | private personal data; **2026-09-15 secret-pattern scan: 0 credential URLs** (only public tzurl.org TZ reference) | feed sha256 equality `9b3f614843cc4d12d6b93a9d4b05f6f3fdd85c457558caf7874e89f0c177f9e9`; re-run URL/token scan at import; iCal structure spot-check | APPROVED — Keep (D4; private gate before remote) |
| M-027 | `Brain/courses/AR173-1P_PLANNING_2/AR173-1P (Fundamentals of Urban Design and Community Architecture)-CLASS SCHEDULE.pdf` @ `e9b231abb898a782da25f7b0e4945f2ea34ad221` | same path | Keep conditional | Fidelity source behind the AR173 schedule | **unclear — university-produced third-party asset; Commander authorization required; private-only; no redistribution** | sha256 equality `e10a43c2f37a9b804f454081248547082a80aa5e074698658daf82a61f4a664f`; manifest entry BEFORE copy; opens/renders check | APPROVED — Keep (D4; private gate before remote) |
| M-028 | `Brain/courses/DSS10_INTRODUCTION_TO_DATA_SCIENCE/SOIT_DSS10_1Q_ Syllabus.docx` @ `29afdeb63a640e8742daa5d20dd04c4a462e6060` | same path | Keep conditional | Syllabus source of truth behind DSS10 | **unclear — university syllabus; Commander authorization; private-only** | sha256 equality `99e388eccc2fc804621fa5cc86cacb157924fed5b88e711a0e1392764dda3fd9`; manifest entry; OOXML opens check | APPROVED — Keep (D4; private gate before remote) |
| M-029 | `Brain/courses/DSS10_INTRODUCTION_TO_DATA_SCIENCE/SOIT_DSS10_1Q_Syllabus.md` @ `b898ec154a213993e83bf4b77044fd4512029dd0` | same path | Keep conditional | Commander-prepared Markdown derivative of M-028; the normal AI-readable layer | derivative of the M-028 third-party asset; same authorization decision; private-only | blob-SHA equality; manifest derivative mapping; visual conversion-fidelity review | APPROVED — Keep (D4; private gate before remote) |
| M-030 | `Brain/courses/GED103_READINGS_IN_PHILIPPINE_HISTORY/GED103 Syllabus_Q12627.docx` @ `e334ab769da48bbb4c6c1682a10e3da7b827f825` | same path | Keep conditional | Syllabus source behind GED103 | **unclear — university syllabus; Commander authorization; private-only** | sha256 equality `eae44c07445f2a48f77aef95d4c78ee40652bca55c0c8141adcb92a061e4c5905a`; manifest entry; OOXML opens check | APPROVED — Keep (D4; private gate before remote) |
| M-031 | `Brain/courses/GED103_READINGS_IN_PHILIPPINE_HISTORY/GED103_Syllabus_Q12627.md` @ `4493e5fc8010da0753786237a822c31c8b3586d4` | same path | Keep conditional | Commander-prepared Markdown derivative of M-030 | derivative of the M-030 third-party asset; same authorization decision; private-only | blob-SHA equality; manifest derivative mapping; plain-domain URL redaction preserved | APPROVED — Keep (D4; private gate before remote) |
| M-032 | `Brain/courses/MEC30-7_STATICS_OF_RIGID_BODIES_FOR_CE/MEC30-7 Course Calendar 1Q.html` @ `66f837c087acfbd322c4a516f3589d6e97f38c60` | same path | Keep conditional | Calendar source behind MEC30-7 | **unclear — university calendar; Commander authorization; private-only** | sha256 equality `495da86995575418f4dd51b67c9e8a2e934c6fdf3bf482b277dc9afeada76af1`; manifest entry; scan for external scripts/trackers | APPROVED — Keep (D4; private gate before remote) |
| M-033 | `Brain/courses/MEC30-7_STATICS_OF_RIGID_BODIES_FOR_CE/MEC30-7_Course_Calendar.md` @ `87be883a25cf0949625868197ed26c0f805585db` | same path | Keep conditional | Pre-existing Markdown derivative of M-032 | derivative of the M-032 third-party asset; same authorization decision; private-only | blob-SHA equality; manifest derivative mapping; visual fidelity review | APPROVED — Keep (D4; private gate before remote) |
| M-034 | `Brain/courses/desktop.ini` @ `d0c6534bef55a9ab063ff473827f988f1f79c152` | — | Exclude | Windows folder metadata; the old manifest itself marks it `exclude_from_ai_ingestion`; references an untracked local screenshot | — | grep confirms absence in v1 | EXCLUDED (D4) |
| M-035 | `Brain/courses/COURSE_CORPUS_MANIFEST.json` @ `ea89ffcce0820c043dfebb43c572cc68487b6199` | Brain/courses/COURSE_CORPUS_MANIFEST.json | Rewrite (rebaseline) | v1 requires a source/hash/permission declaration; the v1 manifest starts EMPTY and gains one entry per approved asset; sha256 recomputed in v1 at import | private declaration file | JSON parse; bidirectional check (every listed file exists with matching sha256; no unlisted file under courses/); policy fields preserved | APPROVED — Rewrite/rebaseline (D4) |
| M-036 | `schemas/course_corpus_manifest.schema.json` @ `0c7b48beb0a8fb16edaa3cf19440d5e0a8d65a87` | — | Exclude v1 (candidate later) | v1 carries no validator machinery; the manifest stands alone and is checked manually; can return in a future bounded validation task | — | manifest manually verified against documented fields at Phase 3 | DEFERRED (D4) |

### Group E — Other personal Brain regions and v3 work products
| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-037 | `Brain/external_sources/` — 13 files (INDEX; books; building-technology; building-utilities; hoa-reviewers; intro-data-science; law; novels; planning; professional-practice; statics-rigid-bodies; structural; toa-reviewers) | — (future per-item corpus candidates) | Exclude v1 | Link lists/notes over copyrighted books and reviewers; selection needs per-item Commander review later | unclear — Commander-authored notes describing in-copyright collections; defer | nothing imported; future items get their own M-IDs with link/license checks | EXCLUDED from v1 baseline (D6; future per-item M-IDs possible) |
| M-038 | remaining `Brain/` — 66 files (`BRAIN_INDEX.md`; cerebellum/; frontal_lobe/ incl. 40 KB task_ledger, testament, opinions, cue notes; temporal_lobe/ session logs; short_term/ ingests, drills, plan; long_term/audits; subsidiary/) | — | Exclude v1 | v3 operating history, cue learning, and session journals — not study-corpus content; cue language may only be rewritten under a separately approved later scope (order §6.2/§9) | private/personal; this is precisely the history v1 leaves behind | grep confirms no frontal_lobe/temporal_lobe/ledger/testament paths in v1 | EXCLUDED from v1 baseline (D6; future per-item M-IDs possible) |
| M-039 | phase work folders `01-research/` … `09-nota/` — 42 files (incl. study-flavored items: PD1096 workshop dossier, planning-law nota cards, `SET-PD1096` drill set + Anki TSV, triangulation worksheets) | — (named future study candidates) | Exclude v1 | Bulk is v3 pipeline state. A handful ARE study material you may later want; they return as individually approved corpus rows, never as a folder copy | mixed; private | nothing imported; future drill/card imports each get an M-ID | EXCLUDED from v1 baseline (D6; future per-item M-IDs possible) |

### Group F — Model research catalog (OPTIONAL — only if you want model comparison in v1)

> Order §6.1: import only if the Commander wants model comparison; every claim
> revalidated against dated sources; never a deployment/routing decision. All
> 14 records are `surface: api`, `region: undeclared`, `retrieved_on 2026-09-15`,
> `review_after 2026-12-14`, and carry self-declared gaps (weak/reserved-domain
> sources for some retention/training strings). **Planner recommendation: defer
> the whole group past v1.0.0.**

| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-040 | `catalogs/model_research/records/anthropic__claude-fable-5-1__api__undeclared.json` @ `82f5acfd641fcdc641a6e2d4185120a4c2621e13` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; carries `supersedes: [anthropic__fable-5-1…]` repair marker; verify supersede chain before any use; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-041 | `catalogs/model_research/records/anthropic__claude-haiku-4-5-20251001__api__undeclared.json` @ `0cf09540ec09e7919b5a77e19ce4d85c7b433319` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-042 | `catalogs/model_research/records/anthropic__claude-opus-5__api__undeclared.json` @ `f7f122ed1019117956530d0d3c47ebcb2729fca0` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-043 | `catalogs/model_research/records/anthropic__claude-sonnet-5__api__undeclared.json` @ `2913566940e66d4d253e983ad24a458dabaa4f62` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-044 | `catalogs/model_research/records/google__gemini-3-1-pro-preview__api__undeclared.json` @ `e5d7df858b71e1b0e8223d5bb84b35b8c0a9341e` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-045 | `catalogs/model_research/records/google__gemini-3-5-flash__api__undeclared.json` @ `22395785a253de920c0e48cf32e1887b90047480` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-046 | `catalogs/model_research/records/google__gemini-3-6-flash__api__undeclared.json` @ `46b7dffb5e6174848573d4dd78d25159a10b5383` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-047 | `catalogs/model_research/records/google__gemini-3-7-flash__api__undeclared.json` @ `1336d3e3195f7ff156133f138e5bc699c416a00d` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-048 | `catalogs/model_research/records/google__gemini-3-8-flash__api__undeclared.json` @ `3c34e1bd5cd6d485d918d78fdacf8464d1572585` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-049 | `catalogs/model_research/records/openai__gpt-5-6-luna__api__undeclared.json` @ `56819e52491a90543a0d96429727415c87fc7d8f` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-050 | `catalogs/model_research/records/openai__gpt-5-6-sol__api__undeclared.json` @ `71e0f470fb6fc11b183a1ddd12981c3a9eca7358` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-051 | `catalogs/model_research/records/openai__gpt-5-6-terra__api__undeclared.json` @ `ea6e6474e2f5ed967ab38c1a3662de6e7595ad28` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-052 | `catalogs/model_research/records/openai__gpt-6-astra__api__undeclared.json` @ `7f59a2fa3c910f5c52ea693bcc711d11adb9a175` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |
| M-053 | `catalogs/model_research/records/xai__grok-4-6__api__undeclared.json` @ `18206e92a790609bf45629699cac273a88b10686` | catalogs/model_research/records/ (optional) | Keep conditional | Structured provider/model research record; research-only, never routing; not revalidated for v1 | internal research notes | JSON parse; every declaration ID bound to the M-054 register; dated primary-source revalidation before any claim is relied on; v1 banner "not revalidated" | DEFERRED past v1.0.0 (D5) |

| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-054 | `catalogs/model_research/sources/REGISTER.json` @ `10670d5001b71e9942f96936edad8736f8a16633`; `catalogs/model_research/sources/SOURCES_2026-09-14.md` @ `4a0c599be8a30fc94bb41451b7ef353e0e4f6f97`; plus 16 receipts `catalogs/model_research/sources/receipts/2026-09-15__O11.md` … `__O26.md` (16 blobs, names only here; full blob list in inspection manifest) | same paths (optional) | Keep conditional | Evidence chain behind the 14 records; records are meaningless without it | internal research; receipts quote dated public web pages | register↔record reference integrity; receipts dated; cited URLs link-tested at revalidation | DEFERRED past v1.0.0 (D5) |
| M-055 | `catalogs/model_research/README.md` @ `8481fbcc73987eac56f10b033baa9e318d67170d`; `catalogs/model_research/INVENTORY.generated.txt` @ `f4cdb5bbf34ffb9943de174488f869aa10b2836a`; `catalogs/model_research/PROPOSAL.md` @ `8410b3ab525cd67aef94632d95342e43f1573721`; `catalogs/model_research/schemas/README.md` @ `a49a3ca097f1bbcdd355afe8ded69d97ad50aa26` | small catalogs/model_research/README.md | Rewrite conditional | If the catalog is adopted, a short v1 README (evidence standard; no-runtime-authority banner) is needed; inventory regenerated only if tooling is later adopted | internal prose | visual review; any inventory count matches the records directory exactly | DEFERRED past v1.0.0 (D5) |
| M-056 | `catalogs/model_research/evals/HARNESS_DESIGN.md` @ `87f87f158bd2fa214e9dde644ce84409646cb9c6`; `catalogs/model_research/decision_matrices/DEPLOYMENT_MATRIX_DESIGN.md` @ `3743ac12be57d91670acaa0a528cae0ec4314b2c`; `schemas/model_research_record.schema.json` @ `e70809227b9fcb00479787730737201908ba46dc`; `schemas/model_research_register.schema.json` @ `036b979538582f1a3130713b0b948087829f3ba1` | — | Exclude | Evaluation harness, deployment matrix, and their machine schemas = routing/evaluation machinery excluded by order §6.3 absent a separate order | — | grep confirms no harness/matrix/deployment content in v1 | EXCLUDED (D5/D6) |

### Group G — v3 machinery, evidence, and history (all Exclude)
| ID | Pinned source path @ blob SHA | Proposed v1 path | Action | Why needed for v1 | Privacy/copyright | Exact verification | Decision |
|---|---|---|---|---|---|---|---|
| M-057 | `scripts/` 20 blobs (incl. validate.py 73 KB, verify_apply.py, cap_probe/cap_verify, feed tooling); `radiation_core/` 3 (control_plane.py + relay.py, 81 KB); `tools/TOOL_REGISTRY.json`; `.github/workflows/` 2 (incl. ical_fetch.yml using `RADIATION_ICS_URL`); `tests/` 5; `evals/` 5 — 36 blobs | — | Exclude | v3 runtime/CI/automation, credentialed automation, and provider-call machinery (order §6.3); no source script was executed during this migration | — | post-build: none of these paths exists in v1; no workflow/credential string present | EXCLUDED (D6) |
| M-058 | `evidence/` 383 blobs (365 task receipt bundles `TID-2026-09-14-*`…`TID-2026-09-15-c`; 17 drafts; 1 control-plane note); `outputs/` 2 (incl. six-point-review) — 385 blobs | — | Exclude | The v3 delivery/gate history v1 deliberately leaves behind; not study material | — | no evidence/ or outputs/ path in v1 | EXCLUDED (D6) |
| M-059 | `scaffolding/` 112 blobs (core procedures; 90 neurons; generated/improved/hosts/control-plane) | — | Exclude | v3 process-rigor machinery; nothing in study-first v1 loads it | — | no scaffolding/ path in v1 | EXCLUDED (D6) |
| M-060 | `styles/` 15; `subskills/` 13; `cue/` 9 (autopilot doctrine, standing directives, lexicon) — 37 blobs | — | Exclude | Deliverable skeletons, passive-subskill system, and the cue engine are v3 OS machinery; cue language returns only after an approved later scope, rewritten (order §6.2/§9) | — | no styles/, subskills/, cue/ paths in v1 | EXCLUDED (D6) |
| M-061 | bulk `docs/` — 39 blobs: AI_RULES, ANTI_PATTERNS, ARCHIVE_NOTES, AUDIT_2026-09-13, BOOT_BUDGET_WAIVERS, CAPABILITIES, CAP_RECORD_POLICY, COMMANDER_QUICKREF, CONTROL_PLANE, CUE_SYSTEM, DECAY_REGISTER, DECISION_AUTHORITY, DEPTH_LADDER, ECOSYSTEM, EVIDENCE_TAXONOMY, KNOWLEDGE_REGISTRY, MODES, OPEN_SOURCES, PATCH_LEDGER, PENDING_RATIFICATIONS, PROMPT_PLAYBOOK, REPLICA_DECISION, ROADMAP, SKILLS, STOCKPILE_DOCTRINE, SYSTEM_STATE, TAXONOMY_MAPPING, THREAT_MODEL, TOOLBOX, WAYFINDING, YIELD_RANKING, examples/×3, shrine/×5 | — | Exclude | The v3 constitution/mode/registry/state apparatus, historical ledgers/audits/shrine; v1 keeps only what Groups A/C rewrite | — | v1 docs/ contains exactly .readme, PROJECT_SCOPE.md, PASS_HANDOFF.md, RELEASE_CHECKLIST.md | EXCLUDED (D6) |
| M-062 | remaining `schemas/` — 13 blobs (cap-record; control-plane ×5; command/event/host-profile/outcome/plan/replica/task-envelope/tool-registry) | — | Exclude | Machine contracts for excluded machinery | — | no schemas/ path unless M-036 is later approved separately | EXCLUDED (D6) |
| M-063 | root `CHANGELOG.md` @ `382309fc8f2541956343a2971d92c79929ee3639` (73,783 B); `.gitattributes` @ `dfe0770424b2a19faf507a501ebfc23be8f54e7b`; `.gitignore` @ `f55ea901808b0173c5e122a40e7edc35fdd173cd` | — | Exclude (all three); a v1 `.gitignore` is handwritten later only if a concrete need appears | v1 history starts afresh at v1.0.0; old release notes are never authoritative v1 history (order §6.3) | — | v1 root carries only the approved file list | EXCLUDED (D6) |

**Coverage check (all 835 pinned blobs):** agents 19 · docs 42 · Brain 100
(courses 21 + external_sources 13 + other 66) · catalogs 38 · phase folders 42 ·
cue/styles/subskills 37 · scaffolding 112 · evidence+outputs 385 · machinery 36 ·
schemas 16 · root 8 = **835**. The per-file blob manifest is held outside the v1
tree at `.inspect/tree_fresh.json` (verified identical to the live GitHub API on
2026-09-15); per-file SHAs for bulk groups are copied into `MIGRATION_LOG.md` if
any such item is ever approved.

---

## 5. Excluded by design — forbidden carrier and red-history families

These are banned from v1 by **name/pattern**, regardless of whether a copy exists
at the pinned snapshot. Filename-pattern scan results over the pinned tree (835
blobs, 2026-09-15):

| Order §2.3 family | Pattern | Hits at pinned fbce71b |
|---|---|---|
| Apply scripts | `APPLY.sh`, `APPLY.ps1` (any path) | **0** |
| Archives | `*.zip` | **0** |
| Patch bundles | `RADIATION_PATCH_*` | **0** |
| Diff files | `PATCH.diff`, `*.diff`, `*_DIFF*` | **0** |
| Append blocks | `append-blocks/`, `append_blocks/` | **0** |
| Staged payloads | `*_STAGED*` | **0** |
| Replacements | `*_REPLACEMENT*` | **0** |
| Old delivery reports | filenames containing "delivery report" | **0** |

Also excluded by design, per order §6.3, even if present anywhere outside the
pinned snapshot (e.g. on the excluded red main, which was **not inspected**):

- the unaccepted **5824 "Release Truth Gate"** implementation and all its
  historical delivery reports — its sole permitted legacy is the short
  `docs/RELEASE_CHECKLIST.md` (M-014);
- **P-11 cue-audit claims, exact rewrites, and the stated "55%" result** until an
  actual external audit and row mapping are supplied and reviewed;
- deployment configuration, provider credentials, external-provider calls,
  automatic routing, model-evaluation results, and legal conclusions;
- current old `main` `e206375783f13216ea9e73b78549517e21d42c09`, as a tree or as
  a version reference;
- any local candidate, ZIP, named branch, or prose report offered as proof of
  public state;
- old CHANGELOG / PATCH_LEDGER content as v1 history.

The Phase 3 receipt re-runs these pattern checks against the actual v1 tree,
fail-closed: any hit blocks the push review.

---

## 6. Privacy / copyright questions for the Commander

| # | Question | Why it matters | Blocked rows |
|---|---|---|---|
| P1 | **Which repository is the target, and is it private?** `CVRadiation` is public today; a fresh `RADIATION-v1` could be created private. | Course material lives only in a confirmed-private repository (order §1/§4) | all of Group D |
| P2 | Authorize storing the four school assets AND their three Markdown derivatives (M-027…M-033) in the **private** v1 repo — personal study, no redistribution? | University-produced third-party material; a checksum is not a permission grant | M-027…M-033 |
| P3 | Confirm personal timetable data (M-024, M-025, M-026) for a **private** study assistant — a fresh decision even though amendment A1 allowed it in the old public repo. | Rooms/sections/class times are personal data | M-024…M-026 |
| P4 | Status of the LMS external-feed **credential rotation** flagged 2026-09-13 (old commit `4a98e59`)? Removing a URL from a tree does not revoke it. | Open security item from old history; v1 should not sit inside an un-rotated secret's blast radius | no file blocked (feed content is clean), but close before any push |
| P5 | Do you want the model-research catalog in v1.0.0, later, or never? | Optional layer; revalidation workload; never a routing input | M-040…M-056 |
| P6 | Later per-item calls on external_sources lists, drill sets, and nota cards (M-037/M-039)? | In-copyright collections referenced; study value but not baseline | future M-IDs |

## 7. Unverified runtime / provider capabilities (v1 must label, not assume)

1. **Folder browsing/selection in hosted products** (ChatGPT, Gemini, Grok,
   Claude): no observation that a pasted repo plus magic words makes any of them
   discover, browse, or choose `agents/<Provider>/`. The v1 `.readme` instructs
   only "if your runtime has opened this repository…" and says so outright.
2. **Arena Agent Mode (this session):** observed here — persistent file
   workspace, shell, web fetch/search; no git push credentials or provider
   accounts used. Observation binds THIS session only.
3. **Dated provider profiles (2026-09-14/15):** carried as dated research with
   the 2026-12-13 review trigger; not refreshed for v1. Status change observed
   2026-09-15: `arena.ai/privacy`, `/terms`, `/pricing` now return HTTP 200 (the
   dated research records 404/reCAPTCHA); page contents unreviewed — the first
   post-v1 profile refresh task.
4. **Model records:** pricing/context/cutoff/retention strings are dated
   declarations from a one-day sweep; some policy strings rest on weak or
   RFC-2606/6761 reserved-domain sources the records themselves flag. No v1 file
   may turn them into compliance or legal conclusions.
5. **PASS handoff:** the v1 card grants nothing; every tool/access field is
   filled from actual session observation or explicitly says "not observed /
   not available".

## 8. Decisions requested (how to approve)

Please answer in plain language; per-ID or per-package both work.

- **D1 — Target repository.** (a) build for a fresh **private** `RADIATION-v1`
  you create *(recommended)*; (b) you flip **CVRadiation to private** and
  designate it the target — its current 50-file early-scaffold tree is then
  treated as data (not a source) and replaced by the approved v1 tree only on
  your explicit order; (c) other (name it).
- **D2 — Privacy gate confirmation** before any Group D copy (API-observed
  visibility is re-checked and recorded at import).
- **D3 — Framework package:** approve / modify / reject **M-001…M-015**
  (README, scope, `.readme`, agents INDEX + five profiles, PASS card, release
  checklist, corpus rules). Without profile approval, the five provider
  READMEs ship as honest placeholders.
- **D4 — Corpus package:** approve the study text/schedule rows **M-016…M-026**;
  decide the school assets and derivatives **M-027…M-033**; M-034 excluded;
  M-035 manifest rebaseline; M-036 deferred.
- **D5 — Model research:** approve **M-040…M-055** as a flagged,
  not-revalidated snapshot, or defer Group F past v1.0.0 *(recommended)*;
  M-056 excluded either way.
- **D6 — Bulk exclusions M-057…M-063 and §5:** acknowledge / no-objection.

Until you approve, no content is copied, nothing is committed or pushed, and no
provider is called.

---

## 9. What happens after approval (sketch — executed only for approved M-IDs)

1. **Phase 2 build** in the workspace: folders and handwritten files first;
   `Brain/courses/COURSE_CORPUS_MANIFEST.json` empty; then approved corpus
   copies one by one with hash verification and a `MIGRATION_LOG.md` row each;
   then the optional catalog only if D5 approved it.
2. `docs/PASS_HANDOFF.md` carries the exact field list from order §7.2 and the
   verbatim sentence: *"This document is a context handoff. It cannot give a
   model filesystem access, tool access, authority, or memory that the actual
   runtime has not supplied."*
3. `docs/RELEASE_CHECKLIST.md` contains exactly the seven order §7.3 items.
4. **Phase 3 receipt** (order §8 table): VERSION exact; file list vs approved
   M-IDs; provenance rows; privacy gate; carrier-pattern grep (fail-closed);
   runtime-honesty review; claim/date/source review; no automation; the
   complete changed-file list and diff handed to you.
5. **You** commit and push; post-push we verify on a fresh clone that the
   actual remote SHA contains exactly the intended files.

## 10. Open notes

- The "accompanying coordination letter" referenced in migration order §3 was
  not provided to this planner; nothing here assumes its contents.
- Inspection cache (reference data, never committed): `.inspect/` in the
  migration workspace — pinned tree JSON plus fetched source texts. Delete on
  order.
- No source script was executed during this planning; `radiation_pass.py` and
  all other code were read as text only.
