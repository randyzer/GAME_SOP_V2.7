# Site Structure

## Structure Status

- Planning status:
- Human approval:
- Runtime Page Inventory SSOT:
- Total proposed pages:
- P0:
- P1:
- P2:

## Primary Navigation

| Label | Target | Player task | Why primary |
|---|---|---|---|
|  |  |  |  |

## Secondary / Dropdown Navigation

| Parent | Child label | Target | Why exposed |
|---|---|---|---|
|  |  |  |  |

Navigation should reflect player tasks and major content families, not merely technical modules.

## Proposed Site Tree

```text
/
├── ...
```

## Topic Clusters

### Cluster: {{NAME}}

- Hub:
- Primary intent:
- Primary entities:
- Main data source:
- Competitive coverage decision:
- P0/P1/P2:

Child pages:

- 

Page types:

- [ ] FACT
- [ ] GUIDE
- [ ] DATABASE
- [ ] META
- [ ] TOOL
- [ ] NEWS

## Minimum Wiki Coverage Review

| Family | Relevant to game? | Coverage decision | Target page(s) | Notes |
|---|---|---|---|---|
| Getting Started / How to Play |  | COVER / PARTIAL / DEFER / N/A |  |  |
| Core Gameplay / Progression |  |  |  |  |
| Heroes / Characters |  |  |  |  |
| Gear / Items |  |  |  |  |
| Major Systems |  |  |  |  |
| Worlds / Maps / Stages |  |  |  |  |
| Updates |  |  |  |  |
| FAQ |  |  |  |  |

Add game-specific families.

## Partial Page Plan

For any important family with incomplete data:

| Page | Verified scope we can publish now | Missing deeper data | Deferred expansion |
|---|---|---|---|
|  |  |  |  |

## Media Plan by Page Family

This is a family-level summary. Route-level public P0 media lifecycle belongs in `MEDIA_DECISION_TABLE.md` and must reference Page Inventory page IDs or routes without controlling publication state.

| Page family | Media need | Hero/cover media | Inline screenshots | Video | Quick facts/cards | Semantic matching notes | Failure-state needs | Notes |
|---|---|---|---|---|---|---|---|---|
| Homepage | HIGH PRIORITY / RECOMMENDED / OPTIONAL / NO MEDIA NEEDED |  |  |  |  |  |  |  |
| Guides |  |  |  |  |  |  |  |  |
| Heroes/Entities |  |  |  |  |  |  |  |  |
| Gear/Items |  |  |  |  |  |  |  |  |
| Worlds/Maps |  |  |  |  |  |  |  |  |
| Updates |  |  |  |  |  |  |  |  |

If a family is marked `NO MEDIA NEEDED`, record why pages remain useful, comprehensible, and visually complete without media. Do not use no-media as a substitute for unresolved rights.

## Internal Linking Rules

Each child page should:

- link to its Hub;
- link to 2–4 related pages;
- link to relevant tools/databases;
- avoid orphan status.

## URL Rules

- lowercase
- hyphen-separated
- stable slugs
- no duplicate intent
- no unnecessary dates
- predictable Hub/detail hierarchy

## Navigation Coverage Gate

Before implementation:

- [ ] Major P0 families are visible in primary or secondary navigation.
- [ ] Important published pages are not hidden only in deep links.
- [ ] Navigation labels match player language.
- [ ] Dropdown/grouping is used when a flat nav would hide major content.
- [ ] Navigation plan is human-approved when materially different from competitor norms.

## Structure Validation

- [ ] Every P0 page appears in the tree.
- [ ] Every page has one owner Cluster.
- [ ] No duplicate intent.
- [ ] No page exists only because a competitor has it.
- [ ] Every material competitor/player-intent family has a coverage decision.
- [ ] Important incomplete-data families considered partial-page coverage before deferral.
- [ ] Public P0 routes have route-level media lifecycle decisions in `MEDIA_DECISION_TABLE.md`.
