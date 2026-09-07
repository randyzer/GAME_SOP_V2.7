# Media Decision Table — v2.6

## Purpose

Classify media needs for public P0 routes and reconcile planned media lifecycle against implementation.

This artifact references the runtime Page Inventory by `pageId` or route. It does not create routes, control navigation, authorize publication, change sitemap/indexability, or replace the Page Inventory SSOT.

## Required Scope

Every public P0 route receives exactly one media need state:

- `HIGH PRIORITY`
- `RECOMMENDED`
- `OPTIONAL`
- `NO MEDIA NEEDED`

`NO MEDIA NEEDED` means the page remains useful, comprehensible, and visually complete without media. It must not mean rights are unresolved.

Do not create media quotas. Text-only and no-media routes are valid when intentional, useful, visually complete, and approved where material.

## Lifecycle States

Media lifecycle:

```text
Media Need
→ Candidate
→ Rights / Human Risk Decision
→ Human Decision
→ Integration
→ Visual Gate
```

Allowed states:

- Media Need: `HIGH PRIORITY`, `RECOMMENDED`, `OPTIONAL`, `NO MEDIA NEEDED`
- Candidate: `NOT FOUND`, `FOUND`, `SEMANTICALLY VERIFIED`
- Rights: `VERIFIED`, `UNRESOLVED`, `HUMAN RISK ACCEPTED`, `NOT REQUIRED FOR EMBED`
- Human Decision: `APPROVED`, `WAIVED`, `REVISE`, `BLOCK`, `PENDING`
- Integration: `NOT INTEGRATED`, `INTEGRATED`, `FALLBACK ONLY`
- Visual Gate: `PENDING`, `PASS`, `REVISE`, `BLOCK`

## Route Decisions

| pageId_or_route | page_family | media_need | need_rationale | intended_placement | candidate_state | rights_state | human_decision | integration_state | visual_gate_state | source_or_provenance | owner_or_defer_reason | notes |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
|  | homepage / hub / guide / static-wiki / update / tool / FAQ / other | HIGH PRIORITY / RECOMMENDED / OPTIONAL / NO MEDIA NEEDED |  | hero / gallery / inline / trailer / diagram / quick-reference / none | NOT FOUND / FOUND / SEMANTICALLY VERIFIED | VERIFIED / UNRESOLVED / HUMAN RISK ACCEPTED / NOT REQUIRED FOR EMBED | APPROVED / WAIVED / REVISE / BLOCK / PENDING | NOT INTEGRATED / INTEGRATED / FALLBACK ONLY | PENDING / PASS / REVISE / BLOCK | first-party / observed / original diagram / source note |  |  |

## Third-party Media Failure State

For embeds, lazy players, unavailable videos, or blocked iframes that would otherwise look broken:

- [ ] Intentional visible fallback exists.
- [ ] Fallback includes useful title/context.
- [ ] Fallback includes source/play/source-link affordance when appropriate.
- [ ] No large blank or broken-looking rectangle remains.

## Blocking Checks

- [ ] Every public P0 Page Inventory route appears here.
- [ ] `HIGH PRIORITY` routes have semantically verified and integrated media or human-approved reclassification/waiver.
- [ ] Homepage `HIGH PRIORITY` media unresolved at Human Visual Review is at least `REVISE` unless Human approves a no-media exception.
- [ ] No selected media is broken, unsourced, rights-blocked, semantically mismatched, or copied from competitors by default.
- [ ] `NO MEDIA NEEDED` routes have intentional composition rationale.
- [ ] `NO MEDIA NEEDED` is not used as a substitute for unresolved rights.
- [ ] Deferred recommended/optional media has owner or defer reason.
- [ ] Third-party media failure states look intentional where blank rendering would look broken.
- [ ] Final implementation reconciles with this table before release.

## Release Notes

- Unresolved high-priority media:
- Human-approved no-media exceptions:
- Human-approved media debt:
- Broken media / delivery warnings:
