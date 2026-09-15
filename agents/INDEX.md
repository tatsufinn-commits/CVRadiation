# AGENT INDEX — RADIATION v1.0.0

Provider-facing routing for runtimes that have already opened **this**
repository. Rewritten for v1 (M-004) from the pinned historical profile index;
the evidence-tier research method (M-010) is embedded below rather than carried
as a separate file. Historical sources, including the old
`agents/RESEARCH_METHOD.md`, exist only inside the inert archive at
`legacy/RADIATION_v3_fbce71b/agents/` (see `docs/LEGACY_BOUNDARY.md`); they are
not live v1 files and grant nothing. v3 scripts and the routing matrix were not
imported into the active layer.

## The routing rule

Read a provider folder **only when your host is explicitly known or observed
to match it**. Unknown, ambiguous, or undeclared host → use the generic
posture below and declare the uncertainty. Never infer a provider from output
style, capability hints, or self-description, and never invent a profile.

| Observed host | Read | Posture in v1 |
|---|---|---|
| Arena Agent Mode session (explicit) | `agents/Arena_AI/README.md` | host session; the PASS card is filled from observation |
| ChatGPT-host session (explicit) | `agents/ChatGPT/README.md` | placeholder; read/plan/draft default |
| Gemini-host session (explicit) | `agents/Gemini/README.md` | placeholder; read/plan/draft default |
| Grok-host session (explicit) | `agents/Grok/README.md` | placeholder; read/plan/draft default |
| Claude-host session (explicit) | `agents/Claude/README.md` | placeholder; read/plan/draft default |
| unknown / ambiguous / undeclared | no provider folder | generic posture: fill `docs/PASS_HANDOFF.md`, declare uncertainty |

## The PASS handoff (all routes)

There is no executable pass in v1. Complete the markdown card at
`docs/PASS_HANDOFF.md`: provider/runtime, observed context, actually available
tools, exposed read paths, task, allowed actions, stop-lines, verification,
known unknowns. The card grants nothing — it records what the host already
supplied.

## Honesty limits (bind this index)

- This index binds only sessions that choose to read it. Repository text
  **cannot make a hosted product auto-discover, browse, or select folders** —
  whether ChatGPT, Gemini, Grok, or Claude do so from a pasted link is
  **unverified as of v1.0.0** and must not be claimed.
- Host label ≠ model identity. No underlying-model claim appears anywhere in
  v1; for Arena Agent Mode model identity is treated as unknowable in-session.
- Observed tools are session evidence only; never generalize one session to a
  platform.
- Read/plan/draft is the default. Commits, pushes, invites, deploys,
  credentials, and external-provider calls are Commander acts.

## Profile status

As of v1.0.0 all five provider READMEs are **placeholders**. The dated
capability profiles and source lists from the pinned snapshot (reviewed
2026-09-14/15, 90-day review trigger 2026-12-13) were **not imported** by
Commander decision D3. Promoting a placeholder to a dated profile requires (a)
a Commander order, (b) the method below, and (c) dated sources.

## Research method for a future profile (retained from M-010)

1. Fresh dated web sweep on a stated date; no claim from model memory alone.
2. Tier every item: **[O]** official primary (provider's own pages/docs),
   **[S]** secondary dated coverage with date, **[U]** user-reported (never
   treated as fact), **[B]** benchmark/independent evaluation (kept separate).
3. Conflicts are recorded as conflicts, never averaged; the official page is
   named as resolution trigger.
4. Missing official surfaces (privacy, terms, pricing, status) are declared
   gaps with review triggers — an invented link is fabrication.
5. Keep surfaces distinct (api / consumer app / enterprise / cloud-managed /
   comparison host); keep region `undeclared` unless a source pins it; every
   volatile claim carries a review date (90-day default).
6. A profile is research notes for the Commander, never authority, never
   routing/deployment input, never a privacy/legal conclusion.
