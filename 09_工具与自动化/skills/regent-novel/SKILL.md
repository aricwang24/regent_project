---
name: regent-novel
description: Manage and write the long-form Chinese novel project 《摄政王·远岬》 by routing canon work, story planning, chapter drafting or revision, character and relationship checks, dialogue work, vehicle and equipment consistency, factual research, continuity review, visual consistency, prose review, and session handoff. Use whenever Codex works on this novel or its repository.
---

# Regent Novel

Use this skill as a lightweight router and source-of-truth guard. Canon, outlines, prose, research and visual assets remain in the repository; do not duplicate them in the skill.

## Locate the project

Find the repository root containing `AGENTS.md` and the numbered directories `00_项目总控/` through `09_工具与自动化/`. Read the applicable root rules and the README of directories that will actually be modified.

If only the connected GitHub repository is available, identify the exact repository and default branch before writing. Prefer a current local checkout when one exists; never assume an unrelated local folder is the project.

Read [references/project-loading.md](references/project-loading.md) and load only the context required by the routed task. Do not automatically load the full story bible, master timeline, all current states, all characters or all review modules.

## Resolve authority

Apply this order:

1. current explicit user instruction;
2. `AGENTS.md` and `00_项目总控/` rules;
3. formal canon in `01_故事圣经/`;
4. formal machine and equipment decisions in `02_机设与装备/`;
5. confirmed plans in `03_大纲/`;
6. occurred facts and current states in `05_连续性管理/`;
7. recent chapters;
8. formal visual guidance in `06_美术资产/`;
9. dated research in `07_参考资料/`;
10. this skill's methods;
11. external examples;
12. model memory.

For conflicts and status labels, read [references/source-priority.md](references/source-priority.md). Report unresolved conflicts instead of silently choosing or filling gaps from old material.

## Route the task

| Intent | Module |
|---|---|
| organize or explicitly revise formal canon | [canon-management](modules/canon-management.md) |
| overall story architecture | [story-architecture](modules/story-architecture.md) |
| unscheduled plot, side story, memory, or character event | [story-pool-management](modules/story-pool-management.md) |
| volume planning | [volume-outline](modules/volume-outline.md) |
| plot-unit planning | [story-architecture](modules/story-architecture.md) |
| chapter brief or outline | [chapter-outline](modules/chapter-outline.md) |
| draft or revise a chapter | [chapter-drafting](modules/chapter-drafting.md) |
| dialogue-focused work or voice calibration | [dialogue-design](modules/dialogue-design.md) |
| character consistency | [character-consistency](modules/character-consistency.md) |
| intimacy, consent, dependency, or relationship boundaries | [relationship-boundaries](modules/relationship-boundaries.md) |
| vehicles, equipment, spatial layout, injury mechanics | [technical-consistency](modules/technical-consistency.md) |
| law, dates, jurisdiction, roads, products, medicine, or other real facts | [factual-research](modules/factual-research.md) |
| image or design continuity | [visual-consistency](modules/visual-consistency.md) |
| timeline, knowledge, state, or cross-chapter audit | [continuity-review](modules/continuity-review.md) |
| tone, narration, pacing, language texture, or AI-pattern review | [prose-review](modules/prose-review.md) |
| end-of-session recovery record | [session-handoff](modules/session-handoff.md) |

Use multiple modules only when the requested work genuinely crosses their boundaries. A local rewrite or scene experiment should remain local.

## Protect formal canon

Modify `01_故事圣经/`, `02_机设与装备/`, or the master timeline only when the user explicitly asks to change formal canon.

- Do not turn a draft, option, archive item or story-pool card into canon.
- Do not alter a character or machine merely to rescue one scene.
- Do not replace locked fictional choices with newly found alternatives without authorization.
- Do not create a second master timeline.
- Put unscheduled ideas in `03_大纲/故事池/` using [templates/story-card.md](templates/story-card.md).

## Normal workflow

1. Identify the requested deliverable, target file and write authorization.
2. Route the task and load the module's minimum current context.
3. Separate locked facts, tentative facts, unknowns and real-world claims only where they matter.
4. Research high-risk real-world facts when needed; do not let research interrupt ordinary fictional details.
5. Produce the requested artifact.
6. Review only the dimensions that could actually make this artifact fail. Do not run the full project checklist on every paragraph, dialogue or local edit.
7. Before promoting prose to `04_正文/`, distinguish a viable formal version from a calibration draft or failed draft. New-book openings and uncalibrated narrative voices default to `08_创作工作区/` until the user explicitly approves the writing voice.
8. Update only files and ledgers that were truly changed.
9. Report unresolved conflicts or blockers without fabricating a resolution.
10. Create a session handoff only for substantial work where later recovery would be useful.

For chapter drafting, follow [modules/chapter-drafting.md](modules/chapter-drafting.md). For artifact writes, follow [references/artifact-update-rules.md](references/artifact-update-rules.md).

## Preserve the reading experience

Default to Fanqie serial manuscript mode while protecting complete emotional, action, dialogue and life processes. Story units may be divided into mobile-readable releases usually around 2,300–3,000 Chinese characters, but this is only a common publishing range. A chapter whose actual content supports about 1,800–2,500 characters should remain short rather than be padded; a complete process may also run longer. Never break or inflate a climax, decisive conversation, core process or ordinary life scene merely to hit a number.

Read [references/fanqie-serial-rules.md](references/fanqie-serial-rules.md), [references/publication-integrity.md](references/publication-integrity.md), and [references/narrative-style-protocol.md](references/narrative-style-protocol.md) only when drafting or revising prose at that scale.

## Finish with evidence

Report what was actually read, changed, checked and left unresolved. Do not claim research, validation, file creation or Git operations that did not occur; do not pad the report with untouched dimensions.