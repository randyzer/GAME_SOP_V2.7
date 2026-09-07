# Source Policy

## Core Rule

**Discovery evidence helps decide what to research, cover, and publish; it does not automatically prove game facts.**

Verification must be evidence-based, not transport-dependent. A failed preferred reader, API, session, CLI, or browser path does not automatically invalidate the underlying evidence.

When a preferred read-only transport fails:

1. classify the access state;
2. preserve the failed attempt;
3. use an approved read-only fallback if available;
4. preserve the same source/provenance identity;
5. verify equivalent evidence before continuing.

Access states:

- `READ`
- `PARTIAL`
- `UNAVAILABLE`
- `TRANSPORT_BLOCKED`
- `AUTH_BLOCKED`

BLOCK only when required evidence itself remains unverifiable.

## Official Sources

Examples:

- official store/site/wiki;
- patch notes;
- developer announcements;
- first-party exposed data.

Allowed for verified facts within their scope.

Label: `official`

## Observed Sources

Examples:

- current game UI;
- screenshots;
- tooltips;
- directly verified gameplay.

Record date/build when possible.

Label: `observed`

## Community Sources

Examples:

- Reddit;
- Discord;
- Steam Discussions;
- YouTube creators;
- repeated player tests.

Allowed for:

- question discovery;
- tips/meta with labels;
- hypotheses;
- practical strategies.

Do not present opinion as official fact.

Label: `community`

## Competitor Sources

Allowed for:

- page-family discovery;
- navigation/UX analysis;
- content-gap analysis;
- candidate questions;
- media/visual-pattern observation;
- intent overlap.

Not allowed as sole factual authority.

Label: `competitor`

## Discovery Evidence

Includes:

- SERP/search suggestions;
- competitor results;
- YouTube;
- community discussion.

Allowed for planning/intent/coverage.

Not allowed by itself for:

- mechanics;
- numbers;
- release/platform claims;
- drop rates;
- hidden mechanics;
- rankings;
- patch behavior;
- unsupported popularity/search-volume claims.

Label: `discovery`

## Media Source Policy

A visual being publicly accessible does not automatically mean it may be freely copied/rehosted.

Prefer:

- first-party official media;
- platform-provided media used within applicable terms;
- directly observed screenshots where appropriate;
- original diagrams based on verified facts.

For game visual identity, prioritize:

1. official key art;
2. Steam capsule;
3. gameplay screenshots;
4. in-game UI;
5. world/map visuals;
6. official trailers;
7. Dev Diary imagery;
8. concept art;
9. publisher marketing-page design only as secondary evidence.

Corporate web color is not game visual identity.

Do not copy competitor-hosted images/videos as a shortcut.

Record media provenance and any known usage constraints.

Also record lifecycle state when media may affect a public P0 route:

- media need: `HIGH PRIORITY`, `RECOMMENDED`, `OPTIONAL`, `NO MEDIA NEEDED`;
- candidate: `NOT FOUND`, `FOUND`, `SEMANTICALLY VERIFIED`;
- rights: `VERIFIED`, `UNRESOLVED`, `HUMAN RISK ACCEPTED`, `NOT REQUIRED FOR EMBED`;
- human decision: `APPROVED`, `WAIVED`, `REVISE`, `BLOCK`, `PENDING`;
- integration: `NOT INTEGRATED`, `INTEGRATED`, `FALLBACK ONLY`;
- visual gate: `PENDING`, `PASS`, `REVISE`, `BLOCK`.

`NO MEDIA NEEDED` means the page remains useful, comprehensible, and visually complete without media. It must not mean rights are unresolved.

Rights/usage notes support human review. They are not an automated legal clearance engine.

## AI Inference

Allowed:

- entity mapping;
- player journey;
- information architecture;
- keyword expansion;
- FAQ candidates;
- partial-page structure;
- prioritization.

Not allowed:

- inventing game facts/numbers/rankings/drop rates/patch behavior.

## Unverified Information

If unverified:

- omit;
- or explicitly label when genuine user value exists.

## v2.6 Partial Page Boundary

A page may exist with incomplete data if every published claim remains properly supported.

Do not confuse:

```text
incomplete dataset
with
permission to invent missing rows
```

and do not confuse:

```text
incomplete dataset
with
automatic prohibition on a useful overview page
```
