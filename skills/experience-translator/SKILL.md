---
name: experience-translator
description: "Translate one real experience into role language for a specific job description. Use when Codex needs to turn a JD and a single project, internship, campus, competition, or personal-product experience into transferable evidence, human interview phrasing, a spoken answer, and reusable experience notes. Do not use for full resume rewrites, broad job matching, or generic interview prep without a single target experience."
---

# Experience Translator

## Overview

Turn one real experience into language the target role can understand. Start from the JD, extract transferable evidence from the experience, and rewrite it into interview-ready phrasing without inventing facts.

## Trigger Guidance

Use this skill when the user asks to:

- turn one experience into role language
- make an experience sound relevant to a specific JD
- write a spoken answer for "tell me about this project"
- save reusable notes for one experience
- reduce AI-like wording in interview talk tracks

Do not use this skill for:

- full resume diagnosis
- full interview question banks
- broad job search advice
- unrelated career planning

## Intake Protocol

Request the minimum useful inputs:

- one target JD or role description
- one experience: project, internship, campus activity, competition, research, or personal product

If the user gives only the experience, ask for the JD before detailed translation. If the user gives only the JD, ask for one experience before writing anything detailed.

## Workflow

1. Extract transferable evidence from the experience.
   - Identify what was actually done, decided, built, improved, or learned.
   - Pull out evidence that could support the target role.
   - Separate confirmed facts from missing details.

2. Map the evidence to JD language.
   - Rephrase the experience using the role's vocabulary.
   - Keep the claim level honest.
   - Prefer concrete actions over abstract ability labels.

3. Generate interview expression.
   - Produce a one-sentence pitch.
   - Produce a spoken version that sounds natural.
   - Produce a short STAR version only if the user needs it.

4. Humanize the answer.
   - Include difficulty, decision points, and real process.
   - Avoid generic phrases such as "responsible for", "strong ability", or "familiar with".
   - Use realistic detail where the material supports it.

5. Save reusable experience notes.
   - Distill the experience into compact notes for future JD adaptation.

## Output Budget

Keep the first response compact.

Default output order:

1. Experience Fit
2. Better Positioning
3. Spoken Version
4. Experience Notes
5. Short next-step chips

Do not expand into full resume advice or a full interview package unless the user explicitly asks.

## Human Interview Style

Prefer spoken language over polished corporate wording.

Do:

- include real difficulty, trade-offs, hesitation, decision points, and process changes
- explain what the candidate actually noticed, tried, adjusted, or learned
- make the answer sound like a real candidate speaking in an interview

Avoid:

- "strong communication skills"
- "responsible for"
- "coordinated and promoted"
- "excellent ability"
- empty labels without a concrete scene

## Experience Notes

Create compact notes for each translated experience:

- Experience label
- Role tags
- Core competency tags
- Confirmed evidence
- Needs-confirmation details
- Reusable pitch
- Spoken version
- Risk note

If the same experience appears again, reuse the existing notes and update only the JD-specific parts.

## Output Standards

Write in the user's preferred language.

Be direct and practical:

- Do not invent metrics, titles, scope, tools, or outcomes.
- Do not overclaim ownership or impact.
- Accept approximate facts only when the user provides the range or basis, such as "about 30-50 people" or "based on the signup sheet". Mark them as approximate instead of precise.
- Prefer plain spoken language over AI-style abstractions.
- Keep the first screen short and actionable.

## Handoff Protocol

- If the experience is too thin, ask 2-3 questions or suggest $story-doctor.
- If the user wants resume wording, hand off to $resume-refiner.
- If the translated experience should be saved or reused, hand off to $experience-bank.
- If the user wants practice, hand off to $mock-interview.

## Suggested Follow-up Chips

End most responses with 2-4 short follow-up prompts that match the current material state.

Examples:

- "改成30秒口语版"
- "补成STAR结构"
- "保存这段经历"
- "再适配一个JD"

If the user asks for final-only output, no chips.
