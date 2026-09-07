# Patch Maintenance SOP

## Trigger

Run when:

- official patch/hotfix lands;
- observed behavior changes;
- market/progression rules change;
- strong community reports suggest verification is needed;
- Search Console changes indicate stale content.

## Workflow

```text
Detect patch
↓
Read official notes
↓
Extract changed systems
↓
Map affected entities
↓
Update fact layer
↓
Find affected Page Inventory rows
↓
Update content
↓
Refresh screenshots/media when UI changed
↓
Update route media lifecycle / visual review evidence when needed
↓
Update verification/freshness
↓
Run targeted QA
↓
Republish
```

## Impact Classes

### High

- progression;
- market;
- hero/skill rework;
- major stats;
- world/stage restructuring.

### Medium

- balance;
- items;
- rewards.

### Low

- cosmetic/UI wording;
- unrelated fixes.

## Meta Review

Balance changes trigger review of:

- Tier List;
- Builds;
- Farming recommendations;
- Skill Tree recommendations;
- endgame guides.

## Partial Page Promotion

A patch or new official dataset may make a formerly partial page ready for expansion.

Review whether:

```text
COVER_PARTIAL
→ COVER_NOW / fuller database
```

## Media Refresh

If patch changes UI, maps, characters, items, or systems shown in screenshots/video:

- mark affected media for review;
- update `MEDIA_DECISION_TABLE.md` media need/candidate/rights/human decision/integration/visual gate states if route media changes;
- refresh `HUMAN_VISUAL_REVIEW_EVIDENCE.md` for affected representative pages;
- avoid visibly stale screenshots on high-value pages.

## Post-Patch QA

Verify:

- changed facts;
- affected pages;
- internal links;
- freshness;
- recommendations;
- media freshness when relevant;
- first-viewport recognition when homepage/UI visuals changed;
- Game Recognition when official visuals, game UI, map/world language, or major media changed;
- semantic media matching when page topics or selected assets changed;
- third-party media fallback states when embeds or players changed;
- template residue and whole-page consistency when layout/theme changed;
- media path, aspect, loading, poster/preload behavior when assets changed.
