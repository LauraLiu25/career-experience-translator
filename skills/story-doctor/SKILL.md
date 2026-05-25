---
name: story-doctor
description: "Mine ordinary or underdeveloped experience for usable career story material. Use when a user says an experience feels too plain, thin, unrelated, or hard to talk about, and Codex needs to ask targeted questions about conflict, choices, changes, constraints, and impact before sending the material to $experience-translator or $resume-refiner. Do not use to fabricate drama, metrics, or achievements."
---

# Story Doctor

## Overview

Help users discover useful story material inside ordinary experience. The goal is not to decorate the story, but to ask better questions until the real difficulty, decision, change, or impact becomes visible.

## Inputs

Need one ordinary experience, even if rough.

Optional:

- Target role/JD
- Current resume bullet
- Interview question the user wants to answer

## Workflow

1. Identify what is missing.
   - Conflict
   - Choice
   - Change
   - Impact
   - Evidence/detail

2. Ask 3-5 targeted questions.
   - Do not ask a long questionnaire.
   - Ask questions that help recover concrete scenes.

3. Extract story elements from the user's answers.
   - Scene
   - Problem
   - Action
   - Decision
   - Result or learning
   - Possible quantification

4. Hand off.
   - Use $experience-translator for interview expression.
   - Use $resume-refiner for resume wording.

## Question Patterns

- Conflict: "Was there any disagreement, constraint, or resource shortage?"
- Choice: "Did you have to choose between two approaches?"
- Change: "What changed after you started?"
- Impact: "What was different because of your work?"
- Detail: "What is one specific moment you still remember?"

## Output Format

1. What may be hidden in this experience
2. Questions to answer
3. Story elements recovered
4. Best next skill to use
5. Suggested next questions

## Standards

- Do not invent stories.
- Approximate facts are acceptable only when the user gives a range or a basis. Keep the uncertainty visible.
- Treat small experiences seriously.
- Prefer concrete scenes over motivational language.

## Handoff Protocol

- Once enough story material is recovered for interview expression, hand off to $experience-translator.
- Once enough evidence is recovered for resume wording, hand off to $resume-refiner.
- If the user uncovers a reusable story, suggest saving it through $experience-bank.
