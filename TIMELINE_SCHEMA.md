# TIMELINE SCHEMA

Timeline records organize life events in chronological order.

The timeline is the backbone of the archive. It should stay factual, structured, and visibly uncertain where needed.

---

# Timeline Entry Fields

Each timeline entry should include:

- Timeline ID:
- Date or Date Range:
- Certainty:
- Age:
- Location:
- Life Era:
- Event Type:
- Summary:
- People Involved:
- Related Places:
- Related Incidents:
- Source:
- Emotional Context:
- Consequences:
- Open Questions:
- Tags:

---

# Event Types

Use one or more:

- birth/family
- home/place
- school
- work
- friendship
- relationship
- health
- loss
- achievement
- conflict
- transition
- identity
- digital-life
- travel
- routine
- belief
- creative-work
- financial
- legal
- other

---

# Timeline Entry Format

```markdown
## [Date or Date Range] - [Short Factual Title]

- Timeline ID:
- Certainty:
- Age:
- Location:
- Life Era:
- Event Type:
- People Involved:
- Related Places:
- Related Incidents:
- Source:
- Tags:

### Summary

Short factual summary.

### Emotional Context

What the user reports feeling or what is clearly documented. Mark uncertainty.

### Consequences

Known short-term and long-term consequences.

### Open Questions

Questions needed to clarify chronology, meaning, people, or consequences.
```

---

# Year File Structure

Timeline files in `archive/timeline/` may be organized by year or range.

Recommended yearly file structure:

```markdown
# Timeline - YYYY

## Year Confidence

- Overall certainty:
- Main locations:
- Main life phase:
- Known anchors:
- Major gaps:

## Entries

Add entries in chronological order.

## Unplaced Memories From This Year

Keep memories that likely belong here but are not yet fixed.

## Open Questions

List questions that would improve the year record.
```

---

# Timeline Integrity Rules

- Do not force an exact date when only a range is known.
- Do not move an entry from approximate to confirmed without source support.
- Do not hide contradictions to make the timeline look clean.
- Do not delete unplaced memories; move them to the appropriate section or working-memory file.
- Every major incident should have both an incident record and a timeline reference.

