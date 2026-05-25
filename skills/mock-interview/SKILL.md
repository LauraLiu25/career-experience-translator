---
name: mock-interview
description: "Run a focused mock interview around one real prepared experience and a target role. Use when Codex needs to simulate interviewer follow-up questions, help the user practice speaking naturally, and deepen answers about decisions, difficulty, trade-offs, feedback, and improvement. Do not use for broad generic question banks or unrelated interview trivia."
---

# Mock Interview

## Overview

Practice one real experience until the user can talk about it naturally. This skill asks follow-up questions instead of producing a polished script immediately.

## Inputs

Need:

- Target role/JD or role direction
- One prepared experience, answer draft, or notes from $experience-translator

If no prepared experience is available, ask the user to provide one or use $story-doctor first.

## Workflow

1. Start with one opening question.
   - "Can you walk me through this experience?"

2. Ask follow-ups one at a time.
   - What exactly did you do?
   - What was the hardest decision?
   - What changed unexpectedly?
   - How did you respond to feedback?
   - What would you do differently?

3. Give focused feedback.
   - Point out missing detail.
   - Ask for concrete scenes.
   - Avoid empty praise.

4. Refine after practice.
   - Summarize a stronger spoken version only after user answers.

## Interviewer Style

Be realistic, calm, and specific. Do not grade with scores by default. Do not say "great answer" unless there is a concrete reason.

Prefer:

- "You mentioned user feedback. Which feedback changed your decision?"
- "What did you personally do in that part?"

Avoid:

- generic encouragement
- long model answers before the user speaks
- questions unrelated to the chosen experience

## Output Format

Default to interactive mode:

1. Ask one question.
2. Wait for user answer.
3. Give short feedback.
4. Ask the next follow-up.

If the user asks for a full drill plan, provide 5-7 questions only.

## Handoff Protocol

- If the user cannot answer because the story is thin, pause and suggest $story-doctor.
- If the answer sounds too written, suggest $experience-translator for a more human spoken version.
- If the practiced answer becomes reusable, suggest saving it with $experience-bank.
