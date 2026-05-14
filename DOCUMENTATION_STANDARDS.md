# DOCUMENTATION STANDARDS

This file defines the repository standards for durable archival writing.

---

# Default Format

Markdown is the default working format.

Use structured sections, metadata blocks, timestamps, tags, references, archive IDs, and internal links.

JSON and YAML are allowed for exports or machine-readable records, but they must be generated from sourced archive material. Structured exports must not introduce new facts.

Recommended Markdown metadata block:

```markdown
## Metadata

- Record ID:
- Record Type:
- Date or Date Range:
- Certainty:
- Source:
- Related Records:
- Tags:
```

Recommended YAML front matter, when useful:

```yaml
record_id:
record_type:
date_range:
certainty:
source:
tags: []
related_records: []
```

---

# Certainty Labels

Use these labels consistently:

- `[Confirmed]` - supported by reliable source material or direct user confirmation.
- `[Approximate]` - likely but not exact, usually a range or estimated placement.
- `[Uncertain]` - remembered or inferred but not stable enough to treat as reliable.
- `[Uncertain Memory]` - memory exists but details, date, or interpretation are unstable.
- `[Incomplete Timeline]` - partial chronological placement is known, but key anchors are missing.
- `[Needs Verification]` - requires follow-up, evidence, or user confirmation.
- `[Conflicting Accounts]` - two or more records disagree.
- `[Inference]` - a reasoned conclusion based on known facts, not direct evidence.

Never remove a certainty label just to make prose smoother.

---

# Date Standards

Prefer ISO-style dates when known:

- `YYYY-MM-DD` for exact dates
- `YYYY-MM` for known month
- `YYYY` for known year
- `YYYY-YYYY` for ranges
- `circa YYYY` for approximate years
- `before YYYY-MM-DD` or `after YYYY-MM-DD` when only relative placement is known

If a date is unknown, write `Unknown` and add an uncertainty label.

---

# File Naming

Use lowercase file names with hyphens.

Recommended patterns:

- incidents: `incident-YYYY-MM-short-title.md`
- timeline years: `YYYY.md`
- timeline ranges: `YYYY-YYYY.md`
- eras: `era-YYYY-YYYY-short-title.md`
- people: `person-name-or-role.md`
- places: `place-name.md`
- digital-life: `digital-YYYY-platform-or-device.md`
- personal profile: `personal-profile.md`
- raw notes: `raw-YYYY-MM-DD-session-or-topic.md`
- sessions: `session-###.md`

If a date is unknown, use:

- `incident-undated-short-title.md`
- `era-undated-short-title.md`
- `raw-undated-topic.md`

---

# IDs

Use stable IDs for cross-reference.

Recommended formats:

- Incident ID: `INC-YYYY-###` or `INC-UNDATED-###`
- Person ID: `PER-###`
- Place ID: `PLC-###`
- Digital Life ID: `DIG-###`
- Era ID: `ERA-###`
- Relationship ID: `REL-###`
- Profile ID: `PRO-###`
- Session ID: `SES-###`

Do not reuse an ID after deleting or merging a record. Instead, mark the original record as superseded.

---

# Linking

Use relative Markdown links.

Examples:

- `../incidents/incident-2010-school-change.md`
- `../people/person-family-member.md`
- `../../working-memory/timeline-gaps.md`

When a relationship is important, link both directions where practical.

---

# Raw Notes

Raw notes preserve the user's source wording.

Do not polish raw notes except for minimal formatting needed to make them readable.

Raw notes may include:
- direct memory fragments
- transcript excerpts
- pasted notes
- document descriptions
- uncertainty as originally expressed

When a raw note becomes an incident or autobiography passage, keep the raw note.

---

# Narrative Writing

Autobiography prose should:
- remain nonfiction
- preserve uncertainty when relevant
- avoid invented dialogue
- avoid invented scenes
- avoid assigning motives without evidence
- keep emotional truth grounded in the user's account
- preserve visible uncertainty when uncertainty affects meaning

Narrative can be elegant. It cannot be false.

Nonfiction craft is allowed for structure, pacing, transitions, and readability. It is not allowed for factual invention.

---

# Revision Notes

Use a revision note when:
- chronology changes
- a contradiction is resolved
- a major fact is corrected
- an event is split or merged
- certainty level changes

Revision note format:

```markdown
## Revision Note
- Date:
- Change:
- Reason:
- Source:
```

---

# Sensitive Material

When writing about private events:
- use neutral language
- distinguish confirmed facts from allegations or interpretations
- avoid unnecessary exposure of third-party private information
- record the user's perspective without treating it as universal fact

The archive should be honest without being careless.
