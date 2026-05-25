---
name: experience-bank
description: "Store, list, search, and reuse compact experience notes created from real career experiences. Use when Codex needs to help a user save experience notes from $experience-translator or $resume-refiner, retrieve relevant experiences for a new JD, or adapt a saved experience to a new role. Do not use as a database unless the user provides or asks to create a local file."
---

# Experience Bank

## Overview

Help the user turn translated experiences into reusable personal assets. This skill is the lightweight storage and retrieval layer for experience notes.

## Inputs

Can work with:

- One experience note to save
- A list of saved notes
- A new JD to match against saved notes
- A request to list, tag, update, or reuse notes

If no storage file is provided, keep the bank in the conversation and offer a markdown table the user can save.

## Experience Note Schema

Use this compact schema:

- ID or label
- Original experience
- Role tags
- Competency tags
- Confirmed evidence
- Needs-confirmation details
- Resume phrase
- Interview phrase
- Risk note

## Operations

Save:

- Convert the current experience output into the schema.
- Ask before writing to a local file.

List:

- Show notes in a compact table.

Search:

- Given a JD or keywords, return the 2-3 most relevant notes.
- Explain why each note matches.

Reuse:

- Hand the selected note to $experience-translator for new JD adaptation.
- Hand the selected note to $resume-refiner for resume polishing.

## Standards

- Do not invent stored history.
- Clearly separate saved facts from new adaptation.
- Preserve approximate numbers as approximate; do not convert them into exact metrics.
- Keep notes short enough to scan.

## Handoff Protocol

- New JD + saved note -> $experience-translator for role-language adaptation.
- Saved note + target resume section -> $resume-refiner for resume wording.
- Saved notes + new JD with many options -> $role-fit-check to choose the best evidence.
