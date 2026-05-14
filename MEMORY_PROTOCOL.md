# MEMORY PROCESSING PROTOCOL

This protocol defines how the agent processes every new memory, note, document, or interview answer.

---

## STEP 0 - SESSION ORIENTATION

Before processing new material:

1. Identify the active session file.
2. Review active investigations, unresolved questions, timeline gaps, and contradictions.
3. Check whether the new material relates to an existing record.
4. Decide whether the material should create a new record, update an existing record, or remain as raw notes until clarified.

If the archive is empty, begin by collecting:
- birth information
- family background
- earliest memories
- main locations
- schools and institutions
- major people
- known timeline anchors

---

## STEP 1 - CAPTURE

Capture raw memory exactly as given.

Do not immediately rewrite heavily.

Store raw notes separately when the memory contains:
- important events
- direct phrasing worth preserving
- emotional detail
- uncertainty
- contradictions
- names, places, or timeline clues

Raw notes belong in `archive/raw-notes/`.

---

## STEP 2 - ENTITY EXTRACTION

Extract:
- dates
- years
- ages
- people
- schools
- workplaces
- locations, houses, neighborhoods, cities, and environments
- emotions
- devices
- online platforms
- usernames or digital identities
- incidents
- transitions
- routines
- identity changes
- consequences
- relationships
- sensory details when supplied by the user
- uncertainty markers in the user's own wording

Do not invent missing entities.

If an entity is implied but not confirmed, mark it as `[Inference]` or `[Needs Verification]`.

---

## STEP 3 - TIMELINE PLACEMENT

Attempt to place memory:
- before or after known events
- inside known life phases
- inside known environments
- near known relationships
- near school, work, city, device, platform, or family anchors
- inside a first chronological skeleton if exact dates are not yet available

Use uncertainty labels:
- `[Confirmed]` for supported dates or facts
- `[Approximate]` for likely ranges
- `[Uncertain Memory]` for unclear or unstable recollection
- `[Incomplete Timeline]` for partial chronology
- `[Needs Verification]` for details requiring confirmation
- `[Conflicting Accounts]` when sources disagree

If placement is impossible, add it to `working-memory/timeline-gaps.md`.

---

## STEP 4 - CROSS-REFERENCE

Connect memory with:
- existing incidents
- people
- places
- emotional phases
- timeline anchors
- life eras
- journals
- autobiography chapters
- digital-life records
- relationship dossiers
- personal profile records
- location history records

Cross-references should use relative links whenever possible.

---

## STEP 5 - INVESTIGATION

If gaps exist, generate targeted follow-up questions.

Good investigation questions are:
- specific
- answerable
- respectful
- anchored to known details
- designed to clarify chronology, people, place, or consequence

Avoid asking too many questions at once.

Ask layered questions when a memory is important:
- chronology anchor
- environment
- people involved
- emotional impact
- consequence
- uncertainty

When a question remains unresolved, record it in `working-memory/unresolved-questions.md`.

---

## STEP 6 - DOCUMENTATION

Create or update:
- incident record
- timeline entry
- autobiography notes
- relationship record
- person record
- place record
- location history record
- digital-life record
- personal profile record
- era record
- contradiction record
- unresolved question
- session log

Use the schemas and templates in this repository.

Default documentation format is Markdown. Use YAML front matter or JSON-style blocks only when they improve structure or exportability.

---

## STEP 7 - REFINEMENT

Continuously improve:
- chronology
- consistency
- readability
- structure
- file organization
- cross-references
- version history
- duplicate detection
- website-readiness when requested

without altering facts.

When refining, keep three layers distinct:

1. Raw source memory.
2. Structured archival record.
3. Narrative autobiography prose.

Never let polished narrative replace source memory.

---

## STEP 8 - SESSION CLOSEOUT

At the end of substantial work:

1. Update the session file.
2. List records created or changed.
3. List timeline anchors discovered.
4. Move unresolved issues to working memory.
5. Record contradictions separately.
6. Identify the next best interview questions.
7. Avoid drafting polished autobiography unless source records are strong enough.

---

# DEFAULT PROCESS FOR A NEW MEMORY

When the user provides a new memory:

1. Briefly acknowledge the memory as source material.
2. Preserve the raw version or identify where it should be stored.
3. Extract known facts and uncertainty.
4. Determine whether it is an incident, timeline entry, relationship update, place note, era note, or autobiography material.
5. Update the correct files.
6. Add revision notes if existing records change materially.
7. Ask only the most useful follow-up questions.

---

# DEFAULT PROCESS FOR A LONG INTERVIEW SESSION

At the end of a session:

1. Create or update the session file in `sessions/`.
2. Add raw notes to `archive/raw-notes/` when needed.
3. Update timeline records.
4. Update or create incident records.
5. Update people, places, eras, or digital-life records.
6. Add contradictions and gaps to working memory.
7. List next investigative questions.
8. Preserve duplicate or alternate versions until they are safely merged or marked superseded.
