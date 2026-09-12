# GAME_SOP V2.6.2 — New Game Wiki Production SOP

A reusable production framework for researching, planning, building, launching, and maintaining SEO-first websites for newly released games.

This repository is the current `GAME_SOP V2.6.2` package. The current
methodology authority is explicitly named
`docs/NEW_GAME_SITE_SOP_v2.6.2.md`. V2.6.1 implementation evidence is
historical provenance archived under `archive/v2.6.1/`; the prior SOP remains
available through Git history. V2.6 artifacts remain under `archive/v2.6/`.
None of these historical materials competes with the current authority.

Version 2.6.2 is a narrow SOP contract release based on the frozen GAME_SOP_v2.6.1 baseline. It preserves the proven methodology while defining **normalized contract-required Pagefind payload semantics** and an explicit **non-final fresh visual evidence-generation lifecycle**. Human Visual `PASS` and final fail-closed closure remain unchanged; D7 remains deferred.

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

## What Changed in v2.6.2

The V2.6.2 additions over the frozen V2.6.1 baseline are:

1. **Pagefind Payload Contract** — the 800,000 B release ceiling applies to normalized contract-required payload, while the raw vendor directory remains diagnostic.
2. **Fail-Closed Artifact Ownership** — Starter owns deterministic Pagefind classification and normalization; optional stock UI already absent is valid, while missing required artifacts and unknown structures block.
3. **Fresh Evidence Build** — `npm run build:evidence` creates explicitly non-final rendered output for Human review without mutating lifecycle authority.
4. **Final Closure Separation** — Human Visual `PASS` remains Human-owned, and evidence output never substitutes for canonical final validation and build.

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
    ├── NEW_GAME_SITE_SOP_v2.6.2.md
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
HUMAN PLANNING APPROVAL
    ↓
FACT LAYER
    ↓
CONTENT + MEDIA IMPLEMENTATION
    ↓
TECHNICAL SEO
    ↓
SCREENSHOT-BACKED HUMAN VISUAL REVIEW + GAME RECOGNITION GATE
    ↓
PLAYER-FACING UX + VISUAL + MEDIA + COVERAGE QA + RECONCILIATION
    ↓
DEPLOYMENT APPROVAL + ACTUAL TARGET VERIFICATION
    ↓
LAUNCH
    ↓
PATCH / SEARCH CONSOLE / COMMUNITY MAINTENANCE
```

## Three Important v2.6 Rules

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
8. Obtain human planning approval.
9. Implement only verified claims; use partial pages and intentional no-media paths when useful and justified.
10. Capture representative rendered screenshots and do not declare V1 complete until `QA_CHECKLIST.md` passes the Game Recognition Gate and media/failure-state checks.
