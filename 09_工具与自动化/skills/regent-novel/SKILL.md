---
name: regent-novel
description: Manage and write the long-form Chinese novel project 《摄政王·远岬》 by routing canon work, story-pool work, overall/volume/chapter planning, chapter drafting or revision, character and relationship checks, vehicle and equipment consistency, factual research, timeline and continuity review, visual consistency, prose review, and session handoff. Use whenever Codex works on this specific novel or its repository, including requests mentioning 摄政王、远岬、林峻、林漪、沈嘉宁、Nico, the Regent project, its outlines, chapters, vehicles, hunting, travel, or continuity records.
---

# Regent Novel

Treat this skill as the project router, context assembler, workflow, and completion gate. Keep canon, outlines, prose, research, and visual assets in the novel repository; do not duplicate them here.

## Locate the project

Find the repository root containing `AGENTS.md` and the numbered directories `00_项目总控/` through `09_工具与自动化/`. Read the applicable `AGENTS.md` and the README of every directory to be touched.

If only the connected GitHub repository is available, identify the exact repository and default branch before reading or writing. Prefer local files when a current checkout exists; keep remote and local contexts aligned. Never assume that an unlinked local folder is the repository.

Read [references/project-loading.md](references/project-loading.md) before assembling context. Load the smallest sufficient set, not the entire story bible.

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

For conflicts and status labels, read [references/source-priority.md](references/source-priority.md). Report unresolved conflicts; do not silently choose a winner.

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
| character consistency | [character-consistency](modules/character-consistency.md) |
| intimacy, consent, dependency, or relationship boundaries | [relationship-boundaries](modules/relationship-boundaries.md) |
| vehicles, equipment, spatial layout, injury mechanics | [technical-consistency](modules/technical-consistency.md) |
| law, dates, jurisdiction, roads, products, medicine, or other real facts | [factual-research](modules/factual-research.md) |
| image or design continuity | [visual-consistency](modules/visual-consistency.md) |
| timeline, knowledge, state, or cross-chapter audit | [continuity-review](modules/continuity-review.md) |
| tone, narration, dialogue, pacing, or AI-pattern review | [prose-review](modules/prose-review.md) |
| end-of-session recovery record | [session-handoff](modules/session-handoff.md) |

Use multiple modules only when the task crosses their boundaries. Fix canon/causality/state problems before sentence-level prose.

## Protect formal canon

Modify `01_故事圣经/`, `02_机设与装备/`, or the master timeline only when the user explicitly asks to change formal canon. Normal planning and drafting never authorize retroactive canon edits.

- Do not make a character act out of bounds to rescue a scene.
- Do not turn a draft, option, archive item, or story-pool card into canon.
- Do not replace locked fictional machine choices with a newly found real-world alternative.
- Do not put a second master timeline under `03_大纲/`.
- Put unscheduled ideas in `03_大纲/故事池/` using [templates/story-card.md](templates/story-card.md).

## Run the workflow

1. Identify the exact deliverable, target file, story stage, and whether writes are authorized.
2. Load project rules, authority files, the relevant outline, the master timeline, current states, and only the involved character/vehicle/visual files.
3. Separate locked facts, tentative facts, unknowns, and real-world claims.
4. Apply the factual research gate. Never guess an A-level fact.
5. Produce the requested artifact with the routed module.
6. Review causality, character, relationship boundaries, technical/spatial logic, time/location, knowledge state, serial readability, and prose.
7. Update only state files that actually changed. Do not mechanically touch every ledger.
8. Record unresolved conflicts or research blockers without fabricating a resolution.
9. Generate a session handoff for substantial work.

For chapter drafting, follow the full checklist in [modules/chapter-drafting.md](modules/chapter-drafting.md). For artifact writes, follow [references/artifact-update-rules.md](references/artifact-update-rules.md).

## Preserve the reading experience

Default to the Fanqie serial manuscript mode with publication-integrity protection. Plan in 20,000–40,000-character story units, then divide into mobile-readable releases usually around 2,300–3,000 Chinese characters. Do not break a complete emotional climax, decisive conversation, or core action merely to hit a count.

Read [references/fanqie-serial-rules.md](references/fanqie-serial-rules.md), [references/publication-integrity.md](references/publication-integrity.md), and [references/narrative-style-protocol.md](references/narrative-style-protocol.md) when drafting or revising prose.

## Finish with evidence

Report files read, files changed, checks run, research sources used, conflicts found, ledgers updated, and remaining blockers. Do not claim research, validation, file creation, or Git operations that did not occur.

