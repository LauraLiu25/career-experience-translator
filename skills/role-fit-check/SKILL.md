---
name: role-fit-check
description: "Evaluate fit between an existing resume/profile and a target JD without reducing the answer to a simple yes/no score. Use when Codex needs to extract JD requirements, identify direct and transferable evidence in a resume, surface gaps honestly, and recommend which experiences should be refined by $resume-refiner or translated by $experience-translator. Do not use for full resume rewriting, interview scripting, or generic career advice without both candidate material and a target role."
---

# Role Fit Check

## Overview

Help the user answer: "Can I apply for this role with my current background?" Focus on evidence, especially transferable experience hidden in non-vertical projects, campus work, part-time jobs, competitions, or research.

## Inputs

Need both:

- Target JD or role description
- Existing resume/profile or experience list

If only the JD is provided, summarize role requirements and ask for resume/profile. If only the resume is provided, give a light readiness note and ask for target roles/JDs.

## Workflow

1. Extract 5-7 JD signals.
   - Separate must-have requirements from bonus signals.
   - Include implied evaluation criteria when visible.

2. Map candidate evidence in three layers.
   - Direct match: same role, tool, domain, or task.
   - Transferable match: different setting but same underlying ability.
   - Gap: no credible evidence in provided material.

3. Translate transferable points.
   - For each strong transferable point, provide one sentence showing how it can be expressed in role language.
   - Keep examples honest and grounded.

4. Recommend next actions.
   - Select 1-2 experiences worth deeper processing.
   - Suggest $resume-refiner for resume wording or $experience-translator for interview expression.
   - If an experience is promising but too thin, suggest $story-doctor first.

## Output Format

Keep output compact:

1. Fit Summary
2. JD Signal Table
3. Evidence Mapping Table
4. Best Transferable Experiences
5. Suggested next questions

Use table columns: JD signal, direct evidence, transferable evidence, gap/risk, next action.

## Standards

- Do not say "low fit" as a dead end. Explain what can and cannot be supported.
- Do not invent experience or data.
- Accept approximate facts only when the user provides the range or basis. Mark them as approximate and ask for confirmation before using them as precise evidence.
- Be honest about gaps without creating panic.
- Prefer "this can be positioned as..." over exaggerated certainty.

## Handoff Protocol

- Strong or transferable experience with enough detail -> $experience-translator.
- Strong resume section that needs better wording -> $resume-refiner.
- Promising but vague experience -> $story-doctor.
- Existing saved notes available -> $experience-bank before choosing experiences.
