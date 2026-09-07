# Content Page Template — v2.6

## Purpose

Standardize player usefulness, SEO, sourcing, internal linking, media richness, and maintenance.

All facts follow `SOURCE_POLICY.md`.
Technical SEO follows `TECHNICAL_SEO_SPEC.md`.

## Page Metadata

```yaml
title:
slug:
pageType: FACT | GUIDE | DATABASE | META | TOOL | NEWS
priority: P0 | P1 | P2
status: draft | published | needs-update
lastUpdated:
lastVerified:
primaryKeyword:
secondaryKeywords:
canonical:
sourceConfidence: official | observed | community | mixed
```

Internal metadata is not automatically public UI.

## Standard Player-Facing Structure

Recommended:

```text
H1
Short intro / quick answer
Relevant hero/cover media when available and semantically matched
Key facts / quick facts
Main task-oriented content
Inline screenshots/video/diagram when useful
Visual rhythm aids where they improve comprehension
FAQ
Related pages
Sources / verification
Last Updated
```

Do not default to exposing:

- internal priority score;
- SEO search-signal labels;
- internal confidence controls;
- internal tags;
- editorial planning instructions.

## GUIDE Pattern

```text
H1
Intro
Quick Answer
Relevant Screenshot / Video
What You Need First
Steps / Mechanics
Common Mistakes
Tips
FAQ
Related Guides
Sources
Last Updated
```

## DATABASE Pattern

```text
H1
Intro
Quick Facts
Representative Media
Filter / Table / List
Entity Details
How Data Works
Related Entities
FAQ
Sources
Last Updated
```

## ENTITY DETAIL Pattern

```text
H1
Entity Image / Visual when available
Entity Summary
Quick Stats
How It Works
Strengths / Uses
Weaknesses / Limits
Unlock / Obtain
Related Build / Gear / Ability
FAQ
Sources
Last Updated
```

## META Pattern

Must include methodology, patch context, evidence type, uncertainty.

## TOOL Pattern

Must contain a real interactive tool before being marketed as a tool.

## Partial Page Pattern

Use when a high-value page intent is real but deep data is incomplete.

Required:

- clearly state verified scope;
- answer the useful part now;
- omit unsupported fields;
- identify major unknowns when relevant;
- do not present a partial page as a complete database.

## Media Rules

Homepage: media required when relevant approved material exists, unless an intentional no-media path is documented and human-approved where material.

Major P0 pages: relevant image/video/media strongly preferred when available.

Route-level media need, candidate, rights, human decision, integration, and visual gate states are tracked in `MEDIA_DECISION_TABLE.md`.

`NO MEDIA NEEDED` means the page remains useful, comprehensible, and visually complete without media. It must not mean rights are unresolved.

For each asset consider:

- source/provenance;
- usage constraints;
- semantic match to the page topic;
- alt text;
- caption;
- optimization.

Do not copy competitor images as a shortcut.

Do not add filler media to satisfy a formula. A text-only page can pass when it is intentional, useful, and visually composed.

Site chrome assets are not page content media. Logos, favicons, header brand marks, and footer marks do not satisfy a content media decision for an article, guide, screenshot, gallery, video poster, or map image.

Third-party media that can fail, delay, or be blocked must have an intentional visible fallback where blank rendering would look broken.

## FAQ Rules

Use real questions from SERP/community/Search Console/YouTube/Steam/Reddit.

3–6 useful questions when appropriate.

## Internal Linking

Every page should link to:

1. parent Hub;
2. 2–4 related pages;
3. relevant tools/databases;
4. related entities.

## Content Quality Checklist

- [ ] Primary player intent is clear
- [ ] No fabricated facts
- [ ] Partial scope is honest where applicable
- [ ] Public UI is player-first
- [ ] Relevant media is used when available
- [ ] Selected media semantically matches the page topic
- [ ] Route media/no-media decision is respected
- [ ] No-media is a positive usefulness/completeness decision, not unresolved rights
- [ ] Third-party media failure state is intentional where relevant
- [ ] Visual rhythm aids improve comprehension without unsupported facts
- [ ] Sources comply with policy
- [ ] Useful internal links exist
- [ ] FAQ contains real questions
- [ ] Last Updated/Verified exists where needed
