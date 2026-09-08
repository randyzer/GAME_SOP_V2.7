# Research Sources

All usage must follow `SOURCE_POLICY.md`.

## Official Sources

| Source | URL | Type | Reliability | Access State | Preferred Transport | Fallback Transport | Allowed Usage | Last Checked | Notes |
|---|---|---|---|---|---|---|---|---|---|
| Store |  | official_store | High | READ / PARTIAL / UNAVAILABLE / TRANSPORT_BLOCKED / AUTH_BLOCKED |  |  | Facts |  |  |
| Website |  | official_site | High |  |  |  | Facts |  |  |
| Wiki |  | official_wiki | High |  |  |  | Facts |  |  |
| Patch Notes |  | official_patch | High |  |  |  | Facts/Updates |  |  |
| YouTube |  | official_video | High |  |  |  | Facts/Demonstration |  |  |

Preserve failed preferred-transport evidence when a fallback verifies the same source. Do not downgrade official evidence to lower-authority evidence silently.

## Official Visual Evidence

Prioritize real game evidence before publisher web styling.

| Source | URL | Evidence status | Identity dimension supported | What it supports | Last checked | Notes |
|---|---|---|---|---|---|---|
| Official key art |  | VERIFIED / OBSERVED / DERIVED / UNAVAILABLE / INTENTIONALLY UNUSED | primary palette / secondary palette / lighting / image style / first-screen |  |  |  |
| Steam capsule |  |  | primary palette / composition / texture-shape language |  |  |  |
| Gameplay screenshots |  |  | UI-material / map-world / semantic media |  |  |  |
| In-game UI |  |  | UI-material / typography / motifs |  |  |  |
| World / map visuals |  |  | map-world / environmental lighting / texture-shape language |  |  |  |
| Official trailer |  |  | lighting / motion / atmosphere / semantic media |  |  |  |
| Dev Diary imagery |  |  | observed systems / production visuals |  |  |  |
| Concept art |  |  | world language / shape language / atmosphere |  |  |  |
| Publisher marketing page |  |  | secondary web-context only |  |  |  |

Corporate web color is not game visual identity.

## Media Asset Inventory

Record assets that may be useful in public pages.

| Asset ID | Type | Source URL | First-party/Observed? | Candidate State | Rights State | Integration State | Visual Gate State | Intended Page(s) / Route Reference | Usage/Rights Note | Alt/Caption Note | Last Checked |
|---|---|---|---|---|---|---|---|---|---|---|---|
|  | key-art / screenshot / video / entity-art / diagram |  |  | NOT FOUND / FOUND / SEMANTICALLY VERIFIED | VERIFIED / UNRESOLVED / HUMAN RISK ACCEPTED / NOT REQUIRED FOR EMBED | NOT INTEGRATED / INTEGRATED / FALLBACK ONLY | PENDING / PASS / REVISE / BLOCK |  |  |  |  |

Do not treat “publicly visible” as automatic permission to copy and redistribute.

Do not copy competitor-hosted images merely because they are easy to access.

This inventory supports media/source decisions but does not replace `docs/MEDIA_DECISION_TABLE.md` or the runtime Page Inventory SSOT.

## Discovery — Web / SERP

| Query | Platform | Page Title | URL | Date | Source Class | Observed Intent | Planning Effect |
|---|---|---|---|---|---|---|---|
|  |  |  |  |  | discovery |  |  |

## Discovery — Competitors

| Competitor/Page | URL | Date | Coverage | Navigation/UX Observation | Media Observation | Planning Effect |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |

## Discovery — YouTube / Community

| Query/Surface | Platform | URL | Date | Source Class | Observed Question | Planning Effect |
|---|---|---|---|---|---|---|
|  |  |  |  | community/discovery |  |  |

## Unsupported / Inaccessible Evidence

Record:

- inaccessible sources;
- network/login/tool limits;
- claims that could not be verified;
- missing first-party visual evidence;
- missing media rights/usage clarity;
- surfaces with no useful evidence.

## Reliability Labels

- `official`
- `observed`
- `community`
- `competitor`
- `discovery`
- `unverified`

## Recording Rule

For factual claims:

```text
source_name
source_url
source_type
source_date
last_verified
confidence
what_it_supports
```

For useful discovery:

```text
query
platform
title
url
accessed_date
source_class
observed_intent_or_question
planning_effect
```
