# RADIATION v1.0.0

**A clean-line, private, study-first repository.**

> - **RADIATION v1.0.0 is a clean-line, private, study-first repository.**
> - **The old RADIATION v3 repository is a read-only reference, not an automatic import source.**
> - **No provider/model claim grants runtime access or authority.**
> - **The Commander approves material imports and performs pushes.**

RADIATION v1 is a small personal study assistant, started clean at v1.0.0. It
is not a copy of the old v3 system and does not claim that v3 content was all
correct. It contains four things:

1. **A provider-facing index** (`agents/`) — one folder per supported AI
   runtime, with an honest routing rule and placeholder profiles.
2. **A bounded PASS handoff** (`docs/PASS_HANDOFF.md`) — a context card that
   states available context, tools, task boundary, stop-lines, and verification
   steps. It grants no access or authority.
3. **A private study corpus** (`Brain/courses/`) — the Commander's enrolled
   courses, schedules, and syllabus materials, imported item-by-item under a
   hash-and-permission manifest.
4. **Migration provenance** (`MIGRATION_SOURCES.md`, `MIGRATION_PLAN.md`,
   `MIGRATION_LOG.md`) — exactly where everything came from and who approved it.

## Quickstart (magic words, v1)

Paste into an AI runtime that already has the repository open:

```text
Read this repository, and act as per docs/.readme
Task: [your study task]
```

A repository text file cannot make a hosted AI browse, select, or obey folders.
If the runtime cannot see this repository, the magic words do nothing — that is
expected, not a bug.

## Layout

```text
RADIATION-v1/
├── README.md                 # you are here
├── VERSION                   # exactly: v1.0.0
├── MIGRATION_SOURCES.md      # what was inspected, what was excluded
├── MIGRATION_PLAN.md         # row-by-row migration decisions (63 M-IDs)
├── MIGRATION_LOG.md          # import ledger: source, hash, reason, privacy, approval
├── agents/                   # provider-facing index
│   ├── INDEX.md
│   ├── ChatGPT/README.md · Gemini/README.md · Grok/README.md
│   ├── Claude/README.md · Arena_AI/README.md
├── docs/
│   ├── .readme               # AI entry gate
│   ├── PROJECT_SCOPE.md      # what v1 is and is not
│   ├── PASS_HANDOFF.md       # bounded context-handoff card
│   └── RELEASE_CHECKLIST.md  # the only release process v1 has
└── Brain/courses/            # PRIVATE study corpus + COURSE_CORPUS_MANIFEST.json
```

## Authority model

- The Commander (repository owner) approves material scope changes, imports,
  and every push. The AI drafts and verifies; it does not commit, push, invite
  collaborators, deploy, route, call providers with credentials, or upload
  material without an explicit, task-bound order.
- Silence, praise, a prior session, or "we are not done yet" is never standing
  approval.
- Claims about providers, policies, models, privacy, or security carry a dated
  source for the relevant surface, or are labelled **not yet verified**.
- Study material lives only in the private repository. No corpus file is
  republished.

Version v1.0.0 means "clean baseline", not "all old features reimplemented".
