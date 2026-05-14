# Life Archive Agent

A long-term autonomous life documentation system designed for Codex and LLM-agent workflows.

Purpose: preserve and reconstruct a real human life through structured interviews, archival investigation, and narrative documentation.

This repository is built for autobiographical work, memory preservation, oral history, personal archival research, and narrative nonfiction documentation.

---

# Core Principles

- truth over drama
- preservation over performance
- investigation over assumption
- emotional honesty over fictional enhancement
- chronology over convenience
- raw source preservation over polished certainty

The archive must remain useful years later. That means every important claim should be traceable, uncertainty should remain visible, and contradictions should be preserved until resolved.

---

# Repository Layout

`AGENT.md` defines the operating identity and behavior of the life documentation agent.

`RULES.md` defines non-negotiable factual, stylistic, privacy, and revision rules.

`MEMORY_PROTOCOL.md` defines how raw memories become structured archival records.

`INTERVIEW_GUIDE.md` defines the interview method and question style.

`DOCUMENTATION_STANDARDS.md` defines naming, date, certainty, linking, and writing standards.

Schema files define durable structures for timelines, incidents, personal profiles, relationships, and life eras.

Location and digital-life schemas define records for places, devices, platforms, online identity, and digital chronology.

`archive/` contains long-term records.

`working-memory/` contains active questions, gaps, contradictions, and current investigations.

`templates/` contains reusable Markdown templates.

`sessions/` contains chronological logs of interview and archival sessions.

---

# Recommended Codex Workflow

Open Codex from the repository root:

```powershell
cd D:\ACTIVE\my\life-archive-agent
codex
```

At the start of each archival session, instruct the agent to read:

1. `AGENT.md`
2. `RULES.md`
3. `MEMORY_PROTOCOL.md`
4. `working-memory/active-investigation.md`
5. `working-memory/unresolved-questions.md`
6. `working-memory/timeline-gaps.md`
7. `working-memory/contradictions.md`

Then provide memories, documents, notes, or interview answers.

---

# Operating Method

For each memory, the agent should:

1. Preserve the raw source.
2. Extract dates, people, places, emotions, and consequences.
3. Place the memory on the timeline where possible.
4. Mark uncertainty explicitly.
5. Cross-reference related records.
6. Ask targeted investigative questions.
7. Update working memory.
8. Refine autobiography material only after the facts are organized.

---

# Privacy Notice

This repository may contain sensitive personal history.

Keep it local unless there is a deliberate reason to share it. Avoid committing private material to public remotes. If this archive is backed up, use a private and controlled storage location.

---

# First Session Prompt

Use this prompt when beginning the archive:

```text
You are working inside the Life Archive Agent repository.

Read AGENT.md, RULES.md, MEMORY_PROTOCOL.md, INTERVIEW_GUIDE.md, DOCUMENTATION_STANDARDS.md, all relevant schema files, and the working-memory files before taking action.

Act as an autonomous Life Archivist Agent. Your task is to document my real life accurately from fragmented memories, conversations, documents, emotions, incidents, and reflections.

Do not invent facts, dialogue, locations, chronology, motives, consequences, or emotional states. Preserve uncertainty honestly. Ask investigative follow-up questions when needed. Keep raw notes separate from structured records and narrative drafts. Preserve contradictions until they are resolved.

Start by reviewing the repository structure, then ask me a small set of high-value questions to build the first chronological skeleton: birth/family background, main places, schools or institutions, earliest memories, important people, and unclear years.
```

For a longer reusable prompt, see `SYSTEM_PROMPT.md`.
