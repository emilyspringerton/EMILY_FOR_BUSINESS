# EMILY_FOR_BUSINESS

## What this is

New repo (2026-09-03), licensing-only so far. See `README.md` for the one-paragraph summary and
`LICENSE.md`/`TRADEMARK.md` for the real legal documents (neither yet reviewed by a lawyer —
each file says so explicitly, don't rely on them as final).

Product scope itself lives in `IDUNA/docs/EMILY_FOR_BUSINESS_NORTHSTAR.md` (S243-02) — a real,
grounded product-scoping pass for the founder's own framing "IDUNA IS THE PRODUCT BASICALLY ZERO
TRUST SECURITY AGENT NATIVE," including a real, direct tension named against IDUNA's own
standing "not a product, it is the backbone" framing, and four open questions for a founder-level
decision that this repo's own future scope depends on. Read that before assuming what belongs
here vs. staying in IDUNA itself.

## Status

Licensing only. No product code yet — real next step (per the NORTHSTAR doc's own "Open
questions") is a founder-level decision on whether this repo becomes a literal externalization of
IDUNA, or a separate product that reuses IDUNA's design.

## The Emily License v0

Custom source-available license (`LICENSE.md`): internal use and modification permitted;
offering the software (or a derivative) as a platform/hosted service to third parties, or
redistributing it, requires a separate commercial agreement. Real, explicit liability cap in
Section 5. `TRADEMARK.md` separately governs the "Emily for Business" name/branding, modeled on
Chef Software's real trademark-policy split (code is one concern, the name is another).

## Related Repos

- `IDUNA` — the real trust-authority backbone this product's own scoping doc is built on;
  `docs/EMILY_FOR_BUSINESS_NORTHSTAR.md` lives there, not here, until the founder resolves
  whether this becomes IDUNA-externalized or a separate product.
- `EmilyOS` — posture-kernel design (`docs/POSTURE.md`), named in the NORTHSTAR doc as an open
  question re: whether it folds into this pitch.
- `EMILY` — RSI loop / backlog coordination for cross-repo work.

## Founder Real-Time Direction

Whenever the founder gives real-time direction — a new ask, a correction, a "can we also..." —
route it through `emily observe -s info "Founder real-time: <summary>"` first, even if it isn't
this repo's usual domain, then sprint-plan it into `EMILY/BACKLOG.md` (`emily backlog curate`,
scoped into a real SECTION/sub-item, not just a one-line log), and only then implement. See
`EMILY/docs/THE_EMILY_WAY.md` Principle 18 ("Pave the Cow Paths").

## Apple Filing Protocol

After any meaningful change, file an Apple:
```bash
emily apples post -t completion -repo EMILY_FOR_BUSINESS "<title>" "<body with commit hash>"
```
Then mark the item done in `EMILY/BACKLOG.md` and commit.

## CHANGELOG Protocol

After any meaningful change, update CHANGELOG.md:
```bash
emily changelog add EMILY_FOR_BUSINESS "<what changed>"
# or manually: append a dated bullet under ## YYYY-MM-DD in EMILY_FOR_BUSINESS/CHANGELOG.md
```

## Frame-Break Reframing

Founder-sourced prompting technique (REDGARDEN/NORTHSTAR.md §28, full origin in
REDGARDEN/docs2/MULTI_AGENT_RD_RESEARCH_NOTES.md §5): given a request, name the underlying
structural/systemic pattern it's one instance of — one level of abstraction up — as an added
lens during planning/triage/judgment calls. Use it to spot the general case behind a specific
ask. It augments judgment, it does not replace doing the work: direct, concrete execution of
the literal task asked for still happens every time.

## Commit Protocol (standing instruction)

Always commit and push completed work immediately — don't wait to be asked. This is the default for every repo in this monorepo.

Every commit — human-written or produced by automated code paths (git-commit helpers in emily-agent, emily.cli, IDUNA handlers, etc.) — must carry the active `emily session` fingerprint as a `session: <tag>` trailer (blank line, then the trailer). This was silently missing from several independently-implemented automated commit helpers across the monorepo until an audit on 2026-08-10 (founder, real-time: "where in the fuck is my llm session id anywhere"). If you add a new automated git-commit code path anywhere, wire in the session tag the same way — don't assume an existing helper already does it.
