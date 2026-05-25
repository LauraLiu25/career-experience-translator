---
name: resume-refiner
description: "Polish an existing resume for a target JD or role without inventing experience. Use when Codex needs to diagnose resume wording, improve JD relevance, reorder or strengthen existing bullets, rewrite selected experience sections, and flag missing evidence. Do not use to create a resume from scratch, fabricate metrics, design visual layouts, or produce interview scripts."
---

# Resume Refiner

## Overview

Improve an existing resume for a specific target role. This skill does not create a fictional resume; it refines what the user already has so the role-relevant evidence is easier to see.

## Inputs

Need:

- Existing resume text or resume file content
- Target JD, role description, or clear job direction

If only a resume is provided, first give a short content/layout diagnosis and ask for the target JD. If only a JD is provided, ask for the resume before candidate-specific edits.

## Workflow

1. Diagnose the current resume.
   - Content strengths
   - Content gaps
   - Wording issues
   - Structure/order issues

2. Extract JD screening signals.
   - Keywords
   - Capability signals
   - Evidence recruiters may scan for

3. Prioritize edits.
   - High priority: role-fit and screening impact.
   - Medium priority: clarity, proof, ordering.
   - Low priority: polish and concision.

4. Rewrite selected bullets.
   - Use action verb + method/context + evidence/result.
   - Preserve truth and seniority.
   - Mark missing metrics as "needs confirmation".

5. Route next step.
   - Suggest $experience-translator for one bullet that needs interview language.
   - Suggest $story-doctor if an experience is too thin to rewrite well.

## Output Format

Default:

1. Quick Diagnosis
2. JD-Relevance Priorities
3. Suggested Edits
4. Sample Bullet Rewrites
5. Missing Facts to Confirm
6. Suggested next questions

Do not rewrite the entire resume unless explicitly asked. Focus on the highest-impact 2-3 sections first.

## Standards

- Never invent data, tools, titles, awards, employers, or outcomes.
- Approximate numbers are allowed only if the user provides a range or basis. Use "about", "approximately", or mark as "needs confirmation"; never turn an estimate into an exact metric.
- Do not make every bullet sound like product/operations if the evidence cannot support it.
- Keep wording professional but not inflated.
- Preserve the user's actual background.

## Handoff Protocol

- If a bullet lacks story detail, use $story-doctor before rewriting aggressively.
- If a revised bullet is likely to be asked in interview, send it to $experience-translator.
- If a refined experience should be reused later, send it to $experience-bank.
