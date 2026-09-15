# PASS HANDOFF — bounded context card (RADIATION v1.0.0)

**Date:** 2026-09-15 · Plan row **M-012/M-015** — concept rewritten from the
pinned v3 `agents/_common/radiation_pass.py` docstring. The old script exists
only inside the inert archive `legacy/RADIATION_v3_fbce71b/agents/_common/` and
was never imported or executed (see `docs/LEGACY_BOUNDARY.md`).

# PROVENANCE NOTE

This card documents a session; it never creates one. **This document is a context handoff. It cannot give a model filesystem access, tool access, authority, or memory that the actual runtime has not supplied.** It is not a privilege grant and not an instruction the host is forced to honour.

## Template

```text
Provider/runtime:            # what you actually observe the host to be;
                             # "unknown/ambiguous" is a valid answer
Observed session context:    # this conversation, the repository mount (if any)
Actually available tools:    # enumerate only tools actually present;
                             # present-but-untested = "present, untested"
Read paths the host has exposed:   # exact paths the runtime can read
Task requested by Commander:
Allowed actions:             # bounded, task-specific
Stop-lines / actions requiring Commander confirmation:
                             # commits, pushes, invites, deploys, credentials,
                             # provider calls, corpus additions, deletions
Verification steps:          # repeatable: command, hash, file list, or dated source
Known unknowns:              # unobserved access, stale-dated claims, etc.
```

## How to fill it honestly

1. **Observation over inference.** A tool in a menu is not a tool you have
   exercised; if untested write "present, untested".
2. **Identity is a label.** A host label never proves an underlying model;
   Arena Agent Mode's underlying model is treated as unknowable in-session.
3. If the repository is not actually mounted/readable in the session, record
   it under Known unknowns and run read-only — do not invent file access.
4. **Stop-line defaults** without an explicit content-bound Commander order:
   no commits, pushes, collaborator invites, deploys, credential use,
   external-provider calls with private data, or corpus additions.
5. Verification must be repeatable: a command, a hash comparison, a file
   list, or a dated source link — not "I checked".
6. An honest "not observed / not available" or "unknown" is a result; papering
   over it is exactly what this card exists to prevent.

## Worked card — the v1 build session (2026-09-15, Asia/Singapore)

```text
Provider/runtime:            Arena Agent Mode (host label from the environment;
                             underlying model identity unclaimed/unknowable)
Observed session context:    Commander migration order + four plan decisions
                             CMD-2026-09-15-D1..D6
Actually available tools:    file workspace (exercised: write/read-back);
                             shell (exercised: curl, python3, hash checks);
                             web fetch/search (exercised: GitHub API, raw
                             blobs, arena.ai status-code probes);
                             git push/credentials: NOT observed, NOT used
Read paths the host has exposed:   /home/user workspace; read-only GitHub
                             API/raw for the pinned commit
Task requested by Commander: inspect RADIATION@fbce71b read-only; bootstrap;
                             row-by-row plan; build approved v1 locally;
                             Commander alone pushes
Allowed actions:             local authoring; read-only inspection; approved
                             local corpus import (D4) with hash verification
Stop-lines honoured:         no git init/commit/push; no source-script
                             execution (including legacy/ archive); zero
                             carrier files in the active layer; visibility is
                             the Commander's decision (public during
                             development per directive 2026-09-15)
Verification steps:          git blob SHA-1 equality (18 verbatim corpus
                             files vs pinned tree); sha256 cross-check (1
                             documented drift: GED103 DOCX); JSON/magic-byte
                             checks; carrier regex scan; final file-list diff
Known unknowns:              folder-browsing in ChatGPT/Gemini/Grok/Claude
                             (unobserved); arena.ai policy/pricing page
                             contents behind 2026-09-15 HTTP 200s (unread);
                             LMS feed credential rotation (Commander item P4)
```

*Note: the v3 PASS was a Python state machine; the v1 PASS is this markdown
card. If a future bounded task adds executable verification, it needs its own
Commander order, source review, and a release-checklist entry.*
