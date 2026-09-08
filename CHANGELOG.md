# Changelog

## 2.6.1

Packaging and SOP hardening release based on frozen `GAME_SOP_v2.6`
provenance. The current V2.6.1 methodology authority is explicitly named
`docs/NEW_GAME_SITE_SOP_v2.6.1.md`.

### Added

- D1 media contract compatibility and deterministic readiness mapping.
- D2 public/internal source boundary.
- D3 runtime evidence contract.
- D4 targeted re-review closure.
- D5 public workflow-language QA.
- D6 production-origin preflight.

### Deferred

- D7 remains deferred.

### Packaging

- Archived the historical V2.6 implementation report under `archive/v2.6/`.
- Archived `archive/v2.6/V2.6_CHANGE_PROPOSAL_V0.2.md` as historical
  baseline/provenance, not current authority.

## 2.6

Production-hardening release based on frozen `GAME_SOP_v2.5` provenance and the approved `V2.6_CHANGE_PROPOSAL_V0.2.md`.

### Added

- Verification Transport Resilience Policy: evidence validity is separate from preferred transport availability.
- Reviewer Capability Preflight before evidence-dependent independent/C2C review.
- First-class Game Recognition Gate in Human Visual Review.
- Official Visual Evidence priority order and planning fields.
- Strongest-competitor visual/media benchmark requirement.
- Complete media lifecycle states for need, candidate, rights/risk, human decision, integration, and visual gate.
- Positive `NO MEDIA NEEDED` definition.
- Third-party media failure-state quality expectation.
- Site chrome vs page content media clarification.
- V2.6 implementation report artifact.

### Changed

- README, SOP, execution prompt, templates, QA checklist, status template, source policy, SEO spec, and patch maintenance now enforce v2.6 evidence/review/visual-media hardening.
- `MEDIA_DECISION_TABLE` now tracks media lifecycle outside the Runtime Page Inventory.
- Human Visual Review now separately records Technical Visual QA, Game Recognition, Visual Identity, Media Density, Semantic Media Matching, Responsive Visual, and Media Failure State.

### Preserved

- GAME_SOP_v2.5 source/provenance discipline.
- KISS, YAGNI, 80/20, High Cohesion, Low Coupling, Modular, Adaptable, Stable Core / Flexible Edge.
- single runtime Page Inventory SSOT.
- Competitive Coverage, Partial Page, Minimum Wiki Coverage, and Navigation Coverage gates.
- no media quotas.
- intentional no-media path.
- no automated legal/copyright/licensing engine.
- no media DAM/CMS/database or generic transport/reviewer/media/visual DSL.
- explicit deployment approval and target verification.

## 2.5

Additive SOP upgrade based on the approved `SOP_V2.5_CHANGE_PROPOSAL.md`.

### Added

- Visual Identity Gate with evidence/status dimensions.
- First-Viewport Game Recognition Gate.
- Route-level `MEDIA_DECISION_TABLE` artifact for public P0 media decisions.
- Media Availability / Resolution Gate.
- Screenshot-backed Human Content / Visual Gate.
- Template Residue Audit.
- Visual Rhythm Gate.
- Whole-Page Visual Consistency Gate.
- Media Performance / Delivery Check.
- `HUMAN_VISUAL_REVIEW_EVIDENCE` artifact for representative rendered screenshots.

### Changed

- README, SOP, execution prompt, templates, QA checklist, status template, content template, source policy, SEO spec, and patch maintenance now enforce v2.5 visual/media release evidence.
- Site Structure keeps media planning at page-family level and points route-level decisions to the media decision table.
- Page Inventory template adds only an external-reference note; no media/layout fields were added.

### Preserved

- GAME_SOP_2.2 source/provenance discipline.
- single runtime Page Inventory SSOT.
- Competitive Coverage, Partial Page, Minimum Wiki Coverage, and Navigation Coverage gates.
- no media quotas.
- intentional no-media path.
- no automated legal engine.
- no universal media byte threshold, CDN, transcoding service, or performance framework.
- explicit deployment approval and target verification.

## 2.2

Production-learning release after the first real site built from the v2.1 workflow.

### Added

- Competitive Coverage Gate
- Competitive Coverage Matrix
- Minimum Wiki Coverage Rule
- Partial Page Rule
- Navigation Coverage Gate
- Media Richness Rule
- Visual Richness Rule
- Player-facing UX Rule
- Planning-to-Implementation Reconciliation
- Version Provenance for SOP / Starter / Master Prompt
- media/source provenance guidance
- stronger release blockers for thin navigation, text-only core pages, and research-metadata-heavy public UX

### Changed

- P0/P1/P2 classification no longer treats incomplete data as an automatic reason to suppress an entire useful page.
- Competitor analysis must produce a decision for each meaningful page family: `COVER_NOW`, `COVER_PARTIAL`, `DEFER`, or `NOT_RELEVANT`.
- Site Structure must include navigation discoverability and media planning.
- QA now evaluates competitive coverage, public information architecture, media richness, and player-facing UX.
- Visual Identity expanded from palette consistency to Visual Identity + Visual Richness.

### Preserved

- official/observed source hierarchy
- single runtime Page Inventory SSOT
- fact-layer discipline
- no fabricated meta/tier/build claims
- KISS/YAGNI/80-20
- explicit deployment approval and target verification
