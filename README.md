# Career Experience Translator

> 经历不是没价值。  
> 只是缺少岗位语言。

Career Experience Translator is a suite of AI Skills for turning real experiences into role-ready resume and interview evidence.

It is designed for candidates who may not have perfectly vertical internships or work experience, but do have real projects, campus work, competitions, part-time jobs, research, or personal products that can be translated into transferable capability evidence.

## What This Suite Does

This suite helps users move through the full career-expression workflow:

```text
story-doctor
dig out story material

role-fit-check
find direct and transferable fit

resume-refiner
polish the existing resume

experience-translator
translate one experience into interview language

mock-interview
practice follow-up questions

experience-bank
save and reuse experience notes
```

## Skills

| Skill | Purpose |
| --- | --- |
| `experience-translator` | Translate one real experience into role language and human interview phrasing |
| `role-fit-check` | Compare a resume/profile with a JD and identify direct or transferable fit |
| `resume-refiner` | Polish an existing resume for a target JD without inventing experience |
| `story-doctor` | Mine ordinary experience for hidden story material |
| `mock-interview` | Practice focused follow-up questions around one real experience |
| `experience-bank` | Store, list, search, and reuse compact experience notes |

## Quick Entry

| If you are stuck here | Start with |
| --- | --- |
| I have a JD but do not know if I can apply | `$role-fit-check` |
| I have a resume and want to polish it for this JD | `$resume-refiner` |
| I have one experience but do not know how to talk about it | `$experience-translator` |
| This experience feels too ordinary | `$story-doctor` |
| I prepared an answer and want to practice | `$mock-interview` |
| I want to reuse old experience notes for a new JD | `$experience-bank` |

## Shared Principles

- Do not fabricate experience, metrics, roles, tools, or outcomes.
- Approximate facts are acceptable only when the user provides a range or basis.
- Keep uncertainty visible with words like "about", "approximately", or "needs confirmation".
- Prefer real details, decisions, constraints, changes, and trade-offs over generic ability labels.

## Repository Structure

```text
career-experience-translator/
├── README.md
├── docs/
│   └── suite-guide.md
└── skills/
    ├── experience-translator/
    ├── role-fit-check/
    ├── resume-refiner/
    ├── story-doctor/
    ├── mock-interview/
    └── experience-bank/
```

Each skill folder contains:

```text
SKILL.md
README.md
agents/openai.yaml
```

