# QA Checklist — v2.6.1

## Purpose

This is the release gate.

A successful build is necessary but not sufficient.

## Content Reliability QA

- [ ] No fabricated game facts
- [ ] Numeric values are sourced
- [ ] P2/meta claims have sufficient evidence
- [ ] Community claims are labeled
- [ ] Competitor-only claims are not treated as facts
- [ ] Partial pages clearly limit their verified scope
- [ ] Patch-sensitive pages show appropriate freshness

## Evidence Resilience QA

- [ ] Required evidence is verified, not merely inferred from preferred tool success/failure
- [ ] Preferred transport failures are classified as `TRANSPORT_BLOCKED`, `AUTH_BLOCKED`, `UNAVAILABLE`, or `PARTIAL`
- [ ] Approved read-only fallback evidence preserves source/provenance identity
- [ ] Primary failure evidence and fallback verification evidence are both preserved
- [ ] No official source was silently downgraded to lower-authority evidence
- [ ] Project is BLOCKED only when required evidence itself cannot be verified

## Reviewer Capability QA

- [ ] Evidence-dependent independent review has reviewer capability preflight
- [ ] Reviewer can access required Git/source/status/execution/build/visual evidence classes
- [ ] Reviewer access gaps are classified as `REVIEWER CAPABILITY BLOCKED`
- [ ] Reviewer capability failures are not mislabeled as project blockers
- [ ] Failed review attempts remain in process history
- [ ] Safe reviewer-readable evidence channel exists before EXECUTED review

## Competitive Coverage QA

- [ ] Competitive Coverage Matrix exists
- [ ] Every material page family has `COVER_NOW`, `COVER_PARTIAL`, `DEFER`, or `NOT_RELEVANT`
- [ ] Material `DEFER` decisions are explained
- [ ] Partial-page coverage was considered before suppressing high-value families
- [ ] Material competitive gaps have human approval

## Minimum Wiki Coverage QA

- [ ] Getting Started / How to Play reviewed
- [ ] Core Gameplay / Progression reviewed
- [ ] Heroes / Characters reviewed
- [ ] Gear / Items reviewed
- [ ] Major Systems reviewed
- [ ] Worlds / Maps / Stages reviewed
- [ ] Updates reviewed
- [ ] FAQ / recurring questions reviewed
- [ ] Game-specific major families reviewed

## Navigation Coverage QA

- [ ] Primary navigation reflects major player tasks
- [ ] Important published families are visible in primary or secondary navigation
- [ ] Important P0 pages are not hidden only in deep links
- [ ] Dropdown/grouping exists when needed
- [ ] Actual navigation reconciles with approved `SITE_STRUCTURE.md`

## SEO QA

- [ ] Unique title
- [ ] Useful meta description
- [ ] Correct canonical
- [ ] One clear H1
- [ ] Internal links exist
- [ ] Breadcrumbs correct where used
- [ ] Structured data matches visible content
- [ ] Sitemap includes intended indexable pages
- [ ] No accidental noindex
- [ ] Hreflang correct if multilingual

## Production Origin Preflight

- [ ] Canonical URLs use the intended production origin
- [ ] Sitemap URLs use the intended production origin
- [ ] `robots.txt` sitemap reference uses the intended production origin
- [ ] No placeholder/example domain remains at final production readiness
- [ ] No `vercel.app` canonical remains when a custom domain is the intended production URL
- [ ] Apex/www choice is explicit and consistent
- [ ] Redirects are consistent with the chosen canonical host
- [ ] Provider/deployment target alone is not treated as public launch proof
- [ ] Live production behavior is inspected before launch is claimed

## Visual Identity QA

- [ ] Official Visual Evidence section exists in `PROJECT_BRIEF.md` or approved planning authority
- [ ] Visual direction derives from real game visuals, not only publisher corporate web colors
- [ ] Official key art / Steam capsule / gameplay screenshots / in-game UI / map-world / trailer evidence were prioritized where available
- [ ] Visual identity dimensions have evidence/status labels in `PROJECT_BRIEF.md`
- [ ] First viewport identifies the specific game and site purpose on desktop and mobile
- [ ] Generic Starter branding is replaced/adapted
- [ ] Template residue is replaced, neutralized, or intentionally retained
- [ ] Core colors are consistent
- [ ] Homepage and internal pages feel like the same game/site
- [ ] Accessibility/readability remains acceptable

## Visual Richness QA

- [ ] Internal pages are not all visually identical text sheets
- [ ] Major page families have appropriate visual hierarchy
- [ ] Cards/tables/quick facts/media blocks are used where they improve game comprehension
- [ ] Representative long-form pages have enough rhythm to scan without formulaic filler
- [ ] Intentional text-only pages remain composed and useful
- [ ] Page-family accents/variants do not become uncontrolled hard-coded styling

## Media Richness QA

- [ ] `docs/MEDIA_DECISION_TABLE.md` exists for new SOP-aligned public P0 routes
- [ ] Root `MEDIA_DECISION_TABLE.md`, if present, is treated only as legacy V2.6 Starter compatibility
- [ ] Root and `docs/` media decision tables do not both exist
- [ ] Every public P0 route has media need/candidate/rights/human decision/integration/visual gate states
- [ ] Lifecycle states use only exact SOP-defined values; unknown values are treated as malformed
- [ ] `pageId_or_route` resolves to exactly one Runtime Page Inventory `pageId` or `route`
- [ ] High-priority media is semantically verified, integrated, and visually accepted or human-reclassified/waived
- [ ] Homepage high-priority media unresolved at Human Visual Review is at least `REVISE` unless Human approves a no-media exception
- [ ] No-media routes have intentional rationale where material
- [ ] `NO MEDIA NEEDED` means useful, comprehensible, and visually complete without media
- [ ] `NO MEDIA NEEDED` is not used to hide unresolved rights
- [ ] Deferred recommended/optional media has owner or defer reason
- [ ] Homepage contains relevant game visual media when available
- [ ] Major P0 guides/hubs include relevant media when available
- [ ] Images/videos have traceable provenance
- [ ] Competitor media is not copied by default
- [ ] Selected media semantically matches the page topic
- [ ] Images have meaningful alt text where appropriate
- [ ] Media is reasonably optimized
- [ ] Video embeds do not break mobile UX
- [ ] Third-party media failure/fallback states look intentional where blank rendering would look broken

## Human Visual Review QA

- [ ] `HUMAN_VISUAL_REVIEW_EVIDENCE.md` exists
- [ ] Screenshots are current and labeled
- [ ] Homepage desktop around 1440px reviewed
- [ ] Homepage mobile around 390px reviewed
- [ ] Representative page families reviewed or marked `NOT APPLICABLE` with Page Inventory evidence
- [ ] At least one whole-page or top/middle/bottom review checks header/body/CTA/media/footer consistency
- [ ] Technical Visual QA is recorded
- [ ] Game Recognition is recorded
- [ ] Visual Identity is recorded
- [ ] Media Density is recorded
- [ ] Semantic Media Matching is recorded
- [ ] Responsive Visual is recorded
- [ ] Media Failure State is recorded
- [ ] First-viewport recognition, template residue, rhythm, media/no-media lifecycle state, and mobile ordering are recorded
- [ ] Human accepted any remaining visual/media debt

## Player-Facing UX QA

- [ ] Public pages lead with player questions/tasks
- [ ] Internal Priority scores are not prominently exposed
- [ ] SEO Search Signal labels are not prominently exposed
- [ ] Internal tags/editorial notes do not dominate public UI
- [ ] Sources/Last Verified are presented in a player-appropriate way
- [ ] Core pages feel like a game wiki/site, not an internal research report
- [ ] Public source rendering uses public-safe fields such as hostname/URL, source type, dates, and neutral link text
- [ ] Internal evidence metadata such as `evidenceNote`, internal reviewer notes, planning evidence, workflow state, or approval state is not rendered by default

## Public Workflow-Language QA

- [ ] Visible public text was inspected for internal workflow/process language that is not meaningful to players/users
- [ ] Internal priority state such as P0/P1/P2 is not exposed as public process status
- [ ] Internal phrases such as planning evidence, Human approval, release approval, later approval, before publication, internal reviewer state, or internal gate state are not leaked as public copy
- [ ] Legitimate editorial uses of release, review, publication, patch, update, priority, or approval are preserved when meaningful in context
- [ ] No naive keyword-ban rewrite was used as a substitute for contextual review

## Planning-to-Implementation Reconciliation

- [ ] Approved Site Structure matches actual public routes
- [ ] Approved Navigation Plan matches actual navigation
- [ ] Approved P0 coverage matches public pages
- [ ] Approved visual/media plan is reflected in core pages
- [ ] Public P0 route media lifecycle matches actual media/no-media/defer states
- [ ] No-media and media deferrals have required human approvals
- [ ] Human Visual Review evidence reflects the current rendered build
- [ ] Any shrinkage/addition is documented and approved

## Page Inventory QA

- [ ] Every live page exists in runtime Page Inventory SSOT
- [ ] P0/P1/P2 state is correct
- [ ] Draft/private content does not leak
- [ ] Navigation/sitemap/search reconcile with Inventory

## Site QA

- [ ] Main navigation works
- [ ] Footer links work
- [ ] No broken internal links
- [ ] No unexpected 404
- [ ] Mobile layout works
- [ ] Required rendered screenshots show no major overlap or blank intended regions
- [ ] Header/body/footer/CTA/media framing feel like one coherent site
- [ ] Tables/media usable on mobile
- [ ] No broken intended media
- [ ] Favicon/basic assets load
- [ ] No obvious console-breaking error

## Performance QA

- [ ] Images optimized
- [ ] Local media paths resolve
- [ ] Media dimensions/aspect behavior preserves layout
- [ ] Lead media eager/lazy loading intent is deliberate
- [ ] Below-fold media loading intent is appropriate
- [ ] Video poster/preload behavior is deliberate where video exists
- [ ] Unusually large local video/media has observed behavior and human approval
- [ ] No severe layout shift
- [ ] No obvious blocking asset issue
- [ ] Core pages load acceptably on mobile

## Launch QA

- [ ] Deployment succeeded
- [ ] Actual deployment target/state verified
- [ ] Canonical uses intended production domain
- [ ] Sitemap loads
- [ ] Robots loads
- [ ] Sitemap and robots sitemap reference use intended production origin
- [ ] No placeholder/example domain remains
- [ ] No `vercel.app` canonical remains when custom domain is intended
- [ ] Apex/www canonical host and redirects are consistent
- [ ] Homepage/important Hubs are indexable
- [ ] Search Console planned/complete

## Required Fix Closure QA

- [ ] Each required `REVISE` item has a recorded required fix
- [ ] Changed evidence was inspected by targeted re-review
- [ ] Targeted re-review produced `PASS` before Human approval closed the item
- [ ] Fix-author self-report was not treated as closure by itself
- [ ] Failed or incomplete targeted re-review attempts remain visible in process history

## Blocking Rule

Launch is blocked by:

- fabricated/unsupported facts;
- materially unapproved competitive-coverage gaps;
- navigation that hides core published families;
- widespread 404/broken mobile;
- wrong canonical/robots/noindex;
- placeholder/example production origin or stale `vercel.app` canonical when custom domain is intended;
- inconsistent apex/www canonical host or redirects;
- unchanged generic Starter identity that conflicts with the game;
- missing or stale required screenshot evidence;
- first viewport that is generic, unrecognizable, or has an empty/broken intended media region;
- technical visual QA that passes while real game recognition fails;
- strongest-competitor useful visual/media support materially ahead without recovery plan, waiver, or justified product/genre reason;
- unresolved high-priority route media without human-approved reclassification/waiver;
- homepage high-priority media unresolved at Human Visual Review without explicit no-media exception;
- broken intended media or media that breaks mobile UX;
- blank/broken-looking third-party media fallback state;
- semantically mismatched selected media;
- major template residue marked `UNRESOLVED`;
- major header/body/footer/CTA/media inconsistency;
- homepage/core experience that is materially text-only despite available approved media;
- public pages dominated by internal research/SEO metadata;
- public pages leaking internal workflow/process language as player-facing copy;
- required `REVISE` item closed without targeted re-review `PASS` and Human approval;
- material mismatch between approved Site Structure/Navigation and actual implementation.
