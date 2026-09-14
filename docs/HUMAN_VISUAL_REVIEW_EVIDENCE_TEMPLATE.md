# Human Visual Review Evidence

## Purpose

Record current rendered screenshot evidence and human review outcomes for technical visual QA, Game Recognition, Visual Identity, Media Density, Semantic Media Matching, Responsive Visual, Media Failure State, template residue, rhythm, mobile ordering, and whole-page consistency.

Use representative evidence, not every route across every viewport.

## Build / Evidence Context

- Project:
- Evidence command: `npm run build:evidence`
- Evidence identity: `NOT FINAL`
- Evidence marker verified: `dist/EVIDENCE_BUILD_NOT_FINAL.json`
- Build URL or local preview:
- Commit/ref if available:
- Review date:
- Reviewer:
- Screenshot folder:
- Page Inventory source:

Evidence-build success creates reviewable output only. It is not canonical build `PASS`, publication authority, media lifecycle authority, or Human approval. It must not mutate lifecycle state. Human review is required before final closure.

## Representative Coverage

If a page family does not exist, mark `NOT APPLICABLE` and reference Page Inventory evidence.

| Page family | Page ID / Route | Desktop evidence around 1440px | Mobile evidence around 390px | Extra viewport if useful | Status | Notes |
|---|---|---|---|---|---|---|
| Homepage |  |  |  |  | PASS / CONDITIONAL PASS / BLOCKED / N/A |  |
| Hub |  |  |  |  |  |  |
| Guide / article |  |  |  |  |  |  |
| Static wiki page |  |  |  |  |  |  |
| Update |  |  |  |  |  |  |
| Tool |  |  |  |  |  |  |
| FAQ |  |  |  |  |  |  |

## First-Viewport Game Recognition

- Literal game identity visible:
- Primary player task / CTA visible:
- Media or intentional no-media composition:
- Desktop result:
- Mobile result:
- Human decision: PASS / CONDITIONAL PASS / BLOCKED

## Game Recognition Gate

Technical Visual QA is necessary but not sufficient.

| Review dimension | Human decision | Evidence / Notes |
|---|---|---|
| Technical Visual QA | PASS / REVISE / BLOCK |  |
| Game Recognition | PASS / REVISE / BLOCK |  |
| Visual Identity | PASS / REVISE / BLOCK |  |
| Media Density | PASS / REVISE / BLOCK |  |
| Semantic Media Matching | PASS / REVISE / BLOCK |  |
| Responsive Visual | PASS / REVISE / BLOCK |  |
| Media Failure State | PASS / REVISE / BLOCK |  |

Required questions:

- Does the site immediately look like this specific game?
- Are real game visual cues materially represented?
- Is the palette derived from the game rather than only corporate web colors?
- Are high-value pages visually supported?
- Are we materially below the strongest competitor in useful visual/media support?
- Are selected images semantically matched to page topics?
- Is no-media an intentional exception?
- Do third-party media failures look intentional rather than broken?

## Template Residue Audit

| Item | Status | Evidence / Notes |
|---|---|---|
| default/demo slogan | REPLACED / INTENTIONALLY RETAINED / NEUTRAL / UNRESOLVED |  |
| default hero composition |  |  |
| generic grid |  |  |
| coordinate rails |  |  |
| unexplained palette |  |  |
| default typography character |  |  |
| repeated generic card patterns |  |  |
| generic marks/icons |  |  |
| large disconnected flat-color regions |  |  |
| footer treatment |  |  |

## Visual Rhythm / Whole-Page Consistency

- Long-form pages reviewed:
- Useful visual aids present where they improve comprehension:
- Text-only pages intentionally composed:
- Header/body/CTA/media/footer consistency:
- Mobile ordering / overlap issues:
- Human decision: PASS / CONDITIONAL PASS / BLOCKED

## Media Delivery Notes

- Broken media:
- Semantically mismatched media:
- High-priority unresolved media:
- Homepage high-priority unresolved media:
- Human-approved no-media exceptions:
- Path issues:
- Dimensions/aspect behavior:
- Lazy/eager loading intent:
- Video poster/preload behavior:
- Third-party fallback state:
- Large local video warnings:

## Human Ads Review (Conditional)

Complete this subsection when monetization is enabled or a release claim depends on provider delivery. Otherwise record `Not applicable — monetization disabled/deferred/unconfigured` and verify zero ad-specific output in QA. This subsection reuses the existing Human Visual/Release outcome; it does not create an ads lifecycle state.

- Applicable and reason:
- Planned semantic placement intent:
- Observed placement(s) by page/locale:
- Provider/project multiplicity evidence:
- Desktop placement/layout/obstruction result:
- Mobile placement/layout/obstruction result:
- Blank/dark-region diagnostic result and owning layer:
- Known-dimension reservation / layout-shift result:
- Ordinary-browser provider check required/performed:
- `REQUESTED` evidence and method:
- `RENDERED` evidence and method:
- `VIEWABLE` evidence, meaningful viewport condition, and method:
- Provider/environment classification, if unresolved: `PROVIDER/ENVIRONMENT CHECK REQUIRED` / `HUMAN_BROWSER_CHECK_REQUIRED` / N/A
- Equivalent-locale semantic intent result and documented exceptions:
- Private credential / internal workflow-language check:
- SEO/UX regression check:
- Evidence / notes:

Do not infer `RENDERED` from a request or `VIEWABLE` from render. An automation error is not production-delivery proof; preserve the limitation and require an ordinary-browser check when the claim matters.

## Final Human Decision

- Overall status: PASS / CONDITIONAL PASS / BLOCKED
- Accepted visual debt:
- Release blockers:
- Required follow-up:
- Human Visual `PASS` recorded by:
- Final closure authorized: YES / NO

After Human lifecycle approval and final reconciliation, run the canonical closing sequence: `npm test`, `npm run validate`, `npm run check`, then `npm run build`. Confirm canonical final output does not retain `dist/EVIDENCE_BUILD_NOT_FINAL.json`.
