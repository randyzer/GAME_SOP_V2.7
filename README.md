# GAME_SOP V2.6.3 — New Game Wiki Production SOP

A reusable production framework for researching, planning, building, launching, and maintaining SEO-first websites for newly released games.

This repository is the current implementation-stage `GAME_SOP V2.6.3` package. The current
methodology authority is explicitly named
`docs/NEW_GAME_SITE_SOP_v2.6.3.md`. V2.6.2 remains the frozen source baseline
and its prior authority remains available through Git history. V2.6.1 implementation evidence is
historical provenance archived under `archive/v2.6.1/`; V2.6 artifacts remain under `archive/v2.6/`.
None of these historical materials competes with the current authority.

Version 2.6.3 is a bounded SOP implementation based on the frozen GAME_SOP_v2.6.2 baseline. It preserves the proven methodology while adding a **provider-neutral monetization and semantic ad-placement contract**, layered layout diagnostics, precise requested/rendered/viewable evidence terminology, and a lightweight conditional Human Ads Review inside the existing Human lifecycle. It does not add Starter mechanics, a provider framework, an ads lifecycle state machine, or runtime analytics.

## Core Principle

**Public Data First → Resilient Evidence Verification → Discovery Research → Competitive Coverage → Structure First → Official Visual Evidence + Route Media Lifecycle → Launch Useful Coverage Fast → Game Recognition Review → Community Refine → Patch Maintain**

The goal is not merely to produce a technically correct site. The goal is to produce a site that is:

- fact-grounded;
- competitive enough to matter;
- easy for players to navigate;
- visually recognizable as a site for the specific game from evidence-backed direction;
- explicit about where screenshots/video/media are high priority, recommended, optional, or positively not needed;
- reviewed with current rendered screenshots and a first-class Game Recognition Gate before release;
- resilient when a preferred read-only transport fails but equivalent evidence can be verified through an approved fallback;
- maintainable after patches.

## What Changed in v2.6.3

The V2.6.3 additions over the frozen V2.6.2 baseline are:

1. **Provider/Placement Separation** — provider-specific bootstrap and public slot identity remain separate from semantic page composition.
2. **Zero-Output and Multiplicity Safety** — disabled or unconfigured placements leave no ad DOM, space, script, or request; slot/key/script reuse requires provider/project evidence.
3. **Semantic Placement and Layout Safety** — stable content anchors and earlier homepage primary placement are soft guidance; known dimensions support responsive reservation without universal blank space.
4. **Evidence and Diagnostics** — requested, rendered, and viewable are distinct claims, and blank/dark regions are diagnosed through DOM/layout layers before provider attribution.
5. **Capability-Aware Human Review** — automation failure is not production-delivery proof; enabled monetization receives a lightweight Human Ads Review within the existing review/release methodology.

## Required Project Artifacts

Before implementation, every real game project must maintain:

```text
docs/
├── PROJECT_BRIEF.md
├── RESEARCH_SOURCES.md
├── KEYWORD_RESEARCH.md
├── COMPETITOR_ANALYSIS.md
├── SITE_STRUCTURE.md
├── MEDIA_DECISION_TABLE.md
├── HUMAN_VISUAL_REVIEW_EVIDENCE.md
└── CURRENT_STATUS.md
```

The implementation must also keep **one authoritative structured runtime Page Inventory SSOT**.

Do not manually maintain a second Page Inventory with competing publication states.

`MEDIA_DECISION_TABLE.md` references Page Inventory `pageId`/routes for media planning and reconciliation only. It does not control route existence, navigation eligibility, sitemap, publication state, or indexability.

## Repository Structure

```text
/
├── README.md
├── CHANGELOG.md
├── PACKAGE_MANIFEST.json
├── archive/
│   ├── v2.6.1/
│   │   └── V2.6.1_SOP_IMPLEMENTATION_REPORT.md
│   └── v2.6/
│       ├── V2.6_CHANGE_IMPLEMENTATION_REPORT.md
│       └── V2.6_CHANGE_PROPOSAL_V0.2.md
├── game.config.example.json
├── 新手必读.md
└── docs/
    ├── NEW_GAME_SITE_SOP_v2.6.3.md
    ├── EXECUTION_PROMPT.md
    ├── PROJECT_BRIEF_TEMPLATE.md
    ├── RESEARCH_SOURCES_TEMPLATE.md
    ├── KEYWORD_RESEARCH_TEMPLATE.md
    ├── COMPETITOR_ANALYSIS_TEMPLATE.md
    ├── MEDIA_DECISION_TABLE_TEMPLATE.md
    ├── HUMAN_VISUAL_REVIEW_EVIDENCE_TEMPLATE.md
    ├── SOURCE_POLICY.md
    ├── SITE_STRUCTURE_TEMPLATE.md
    ├── PAGE_INVENTORY_TEMPLATE.md
    ├── P0_P1_P2_TEMPLATE.md
    ├── FACT_DATABASE_SCHEMA.md
    ├── CONTENT_PAGE_TEMPLATE.md
    ├── TECHNICAL_SEO_SPEC.md
    ├── QA_CHECKLIST.md
    ├── PATCH_MAINTENANCE_SOP.md
    └── CURRENT_STATUS_TEMPLATE.md
```

## Production Flow

```text
PROJECT_BRIEF + VERSION PROVENANCE
    ↓
OFFICIAL SOURCE VERIFICATION WITH TRANSPORT RESILIENCE
    ↓
DISCOVERY RESEARCH
    ↓
COMPETITOR ANALYSIS
    ↓
COMPETITIVE COVERAGE GATE
    ↓
KEYWORD / ENTITY / PLAYER-JOURNEY MODEL
    ↓
SITE_STRUCTURE
    ↓
MINIMUM WIKI COVERAGE + NAVIGATION COVERAGE GATES
    ↓
RUNTIME PAGE INVENTORY + P0/P1/P2
    ↓
OFFICIAL VISUAL EVIDENCE + ROUTE MEDIA LIFECYCLE
    ↓
MONETIZATION DECISION + SEMANTIC PLACEMENT INTENT (WHEN APPLICABLE)
    ↓
HUMAN PLANNING APPROVAL
    ↓
FACT LAYER
    ↓
CONTENT + MEDIA IMPLEMENTATION
    ↓
TECHNICAL SEO
    ↓
SCREENSHOT-BACKED HUMAN VISUAL REVIEW + GAME RECOGNITION GATE + CONDITIONAL HUMAN ADS REVIEW
    ↓
PLAYER-FACING UX + VISUAL + MEDIA + COVERAGE QA + RECONCILIATION
    ↓
DEPLOYMENT APPROVAL + ACTUAL TARGET VERIFICATION
    ↓
LAUNCH
    ↓
PATCH / SEARCH CONSOLE / COMMUNITY MAINTENANCE
```

## Four Important v2.6 Rules

### 1. Incomplete evidence does not automatically cancel a page

Bad default:

```text
No complete node database
→ no Skill Tree page
```

Preferred:

```text
Skill Tree system is verified
→ publish a useful Skill Tree overview/guide with verified claims only
→ defer node-level database until evidence is complete
```

**Page existence and claim completeness are separate decisions.**

### 2. A transport failure is not automatically an evidence failure

Bad default:

```text
Preferred reader failed
→ evidence is invalid
→ project BLOCKED
```

Preferred:

```text
Preferred read-only transport failed
→ classify transport/auth/session failure
→ use an approved read-only fallback
→ preserve both failure and fallback evidence
→ continue if equivalent evidence verifies
```

**Evidence validity and transport availability are separate decisions.**

### 3. A technically correct site can still fail the release gate

A site may build successfully and still be unacceptable if:

- major competitor/player-intent families are missing without approved reason;
- navigation hides major published content;
- core pages are text-only despite available relevant media;
- public P0 routes have no media decision or unresolved high-priority media;
- homepage first viewport is generic, unrecognizable, or an empty hero shell;
- technical visual QA passes but real game recognition fails;
- the homepage looks like a game site but internal pages look like generic documents;
- useful visual/media support is materially below the strongest competitor without recovery plan, waiver, or justified product reason;
- screenshots are missing/stale for required human visual review;
- third-party media failure states look blank or broken;
- internal SEO/research metadata dominates the public UI.

### 4. Ad code is not proof of ad delivery or viewability

```text
AD CODE EXISTS != AD IS RENDERED != AD IS VIEWABLE
```

When monetization is disabled or unconfigured, the correct output is no ad wrapper, provider container, reserved space, provider script, or provider request. When enabled, semantic placement stays separate from provider specifics, and provider/environment failures in automation are handed to ordinary-browser review when the delivery claim matters.

## Reliability Rules

Always distinguish:

- **Confirmed Fact** — first-party/official evidence.
- **Observed** — directly verified in the current build/UI.
- **Community Strategy** — player testing/opinion with appropriate labels.
- **Discovery Evidence** — useful for intent, gaps, coverage, and questions.
- **Unverified** — not publishable as fact.

Never fabricate:

- stats;
- drop rates;
- codes;
- tier rankings;
- best builds;
- market rules;
- hidden mechanics;
- patch behavior.

## Quick Start

1. Copy `game.config.example.json` to the real project or translate its fields into the Starter's config.
2. Record the exact SOP / Starter / Master Prompt baseline in `PROJECT_BRIEF.md`.
3. Run official-source verification with transport resilience and bounded Discovery Research.
4. Complete competitor analysis, including the visual/media benchmark, and the Competitive Coverage Matrix.
5. Build Site Structure and a single runtime Page Inventory.
6. Run the Minimum Wiki Coverage and Navigation Coverage gates.
7. Derive Official Visual Evidence, Game Recognition intent, and route media lifecycle decisions.
8. Decide whether monetization is disabled, deferred, or enabled; if enabled, record semantic placement intent, provider/public-private boundary, multiplicity evidence, and locale exceptions.
9. Obtain human planning approval.
10. Implement only verified claims; use partial pages and intentional no-media paths when useful and justified.
11. Capture representative rendered screenshots and do not declare V1 complete until `QA_CHECKLIST.md` passes the Game Recognition Gate, media/failure-state checks, and conditional Human Ads Review.
