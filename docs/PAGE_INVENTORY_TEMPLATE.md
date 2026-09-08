# Page Inventory

## Purpose

Define the conceptual fields and rules for the site's authoritative publication ledger.

The **structured runtime Page Inventory is the SSOT**.

This Markdown file is a schema/planning reference only.

## Suggested Conceptual Fields

| Field | Purpose |
|---|---|
| pageId | stable identifier |
| route | canonical internal route |
| pageType | FACT/GUIDE/DATABASE/META/TOOL/NEWS |
| cluster | owner topic cluster |
| phase | P0/P1/P2 |
| coverageMode | full / partial / deferred |
| visibility | public/private |
| publicationStatus | planned/draft/published |
| contentStatus | research/draft/ready |
| developmentStatus | not-started/building/ready/blocked |
| indexability | index/noindex/not-public |
| primaryKeyword | primary intent wording |
| relatedPageIds | internal-link graph |
| sources | evidence records |
| updatedAt | freshness |
| needsReview | review flag |
| needsUpdate | patch/content update flag |

Implementations may use different exact names; do not add fields solely to satisfy this template if the Starter uses another stable schema.

## Runtime SSOT Rules

- Every planned page exists once in the runtime Inventory.
- Every deployed page exists there.
- P0/P1/P2/visibility/indexability must reconcile with it.
- Draft/private rows must not leak into navigation, sitemap, rendered HTML, or search unless explicitly enabled.
- Do not create a second manually maintained publication ledger.
- Media lifecycle decisions may reference `pageId` or `route` externally in `docs/MEDIA_DECISION_TABLE.md`, but media/layout/lifecycle fields do not belong in the Inventory unless a future architecture review separately approves them.

## v2.6 Coverage Rule

The Inventory may represent a **partial page** as a real page when it safely answers an intent with verified scope.

Do not create a fake “complete database” status for an incomplete reference.

## Human-Readable View Rule

If a Markdown view is useful, generate it one-way and mark it generated.

`SITE_STRUCTURE.md` and `CURRENT_STATUS.md` explain decisions but do not control runtime publication.
