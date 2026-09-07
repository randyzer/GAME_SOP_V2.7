# Fact Database Schema

## Purpose

Define a lightweight reusable fact layer before facts are reused across pages/tools/databases.

**Collect once → structure once → reuse everywhere.**

Use the simplest sufficient implementation.

## Common Provenance Fields

```text
id
name
slug
source
source_url
source_type
source_date
last_verified
confidence
notes
```

Confidence:

```text
official
observed
community
unverified
```

## Common Entity Families

### Hero / Unit

```text
id
name
slug
role
class
rarity
rank
level_cap
abilities
stats
tradable
unlock_method
provenance...
```

### Ability / Skill

```text
id
name
slug
type
description
max_level
effects
cooldown
duration
compatible_entities
unlock_method
provenance...
```

### Gear / Item

```text
id
name
slug
type
slot
set
rarity
attributes
stats
upgrade_cap
tradable
soulbound
obtain_method
drop_sources
drop_rate
provenance...
```

Never fill `drop_rate` without reliable evidence.

### World / Map / Stage

```text
id
name
slug
order
description
unlock_requirement
difficulty
stage_count
bosses
key_items
recommended_level
provenance...
```

### Skill Tree

```text
id
name
slug
branch
tier
level
cost
prerequisites
effect
unlock_requirement
provenance...
```

### Market

```text
id
item_id
market_url
tradable
lowest_price
median_price
listing_count
currency
snapshot_time
provenance...
```

Market snapshots require `snapshot_time`.

### Patch

```text
id
patch_date
patch_version
title
summary
systems_affected
changes
affected_entities
affected_pages
source_url
last_verified
```

### Community Question

```text
id
question
normalized_question
system
platform
source_url
first_seen
last_seen
occurrence_count
candidate_page
candidate_faq
confidence
```

## Storage Recommendation

Small V1:

```text
JSON / typed project object
```

Research:

```text
CSV / spreadsheet
```

Larger proven need:

```text
database
```

Do not introduce a database too early.
