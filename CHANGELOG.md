# Changelog

## 2026-09-11
- docs: new, real, spec-only `docs/UNIVERSAL_UI_NORTHSTAR.md` -- the frontend half of the sharpened Emily For Business platform pitch. Founder real-time: "we need a super abstract language for affordances like a BA would write a user can do this... like react native but even more abstract -- like we target ratatui and android native and react native and flutter and everything you just need to write an adaptor." Names honestly why this is harder than React Native/Flutter (both commit to one GUI-widget-tree paradigm; a terminal is a categorically different one), grounds the idea in this monorepo's own proven "one source, many real target emitters" pattern (PARENA's own C/Java/TS backends, KARAMBIT/SPIDERBEETLE's "PARENA owns decision logic, thin native host does I/O" split as the direct Adapter precedent), proposes a 3-layer model (Affordance IR / Capability Model with mandatory explicit degradation / per-target Adapters), names 5 real open design questions, and a 4-phase plan proving the hardest target pair first. No name locked in, no repo created, no code. CLAUDE.md updated (Status + Related Repos). (sess-20260905-0720-ec33e7c5)

## 2026-09-03

- Repo created (upstream pre-created empty, pulled in this session). New `LICENSE.md` ("The
  Emily License v0" — real, custom, source-available: internal use/modification permitted,
  offering as a platform or redistributing requires a separate commercial agreement, real
  explicit liability cap in Section 5) and `TRADEMARK.md` (separate name/branding policy, modeled
  directly on Chef Software's real code-license-vs-trademark-policy split). Neither reviewed by a
  lawyer yet — both files say so explicitly. Founder real-time direction across two follow-ups:
  "can we write a license based on the chef license?" (real research found Chef's own code is
  actually Apache 2.0 plus a separate trademark policy — not source-available in the BSL/Elastic
  sense — so the Chef model was applied to the trademark half specifically, per founder decision
  after being asked); then "write that emily for business cant be offered as a platform and also
  we need to limit our own liablility... write The Emily Licens v0" — both incorporated directly
  (Section 2.1's explicit "as a platform" restriction, Section 5's explicit liability cap).
  (sess-20260902-2008-ed50169e)
