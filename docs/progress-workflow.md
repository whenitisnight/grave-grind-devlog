# Documentation process

I want this portfolio to explain decisions and their consequences as development progresses. Publication follows major milestones, meaningful problem resolutions, significant architectural pivots, completed features and explicit decisions to log work publicly.

Related commits belong in the relevant entry. Routine edits remain in Git history, keeping the library focused on substantial progress.

## Editorial approach

Each entry starts with a goal or problem, then explains the technical decision, mechanism, reasoning, evidence and remaining limits. The record describes what actually happened and distinguishes planned behavior from implemented results.

I write from the project owner’s perspective. First person establishes decisions, priorities, tradeoffs and judgments. Technical explanations then follow the subject of the work: the camera, collision model, build pipeline or measured result. This keeps ownership clear while allowing connected prose and varied sentence structure.

Headings name topics directly. An entry should read as an authored engineering account, with no chat narration, repetitive status-report phrasing or invented claims of personal testing.

## Problems, lessons and the next approach

I want the library to explain how the process improves, including where an assumption failed or a tool made verification harder. Significant case studies now include the problems encountered, what the evidence taught me, and the concrete change to the next approach.

Each retrospective connects an observed problem to its consequence and the evidence that revealed it. The explanation separates demonstrated causes from hypotheses, then names a practical adjustment: a better acceptance criterion, a smaller reproduction, a clearer build boundary or a more focused review.

Lessons belong beside the decisions they inform. Related earlier cases are linked rather than repeated in full. When a pass finds no new gameplay defect, the entry says so; a retrospective does not require an invented failure or a claimed time saving.

## Library structure

| Location | Purpose |
| --- | --- |
| README.md | Project introduction, current status and navigation. |
| CHANGELOG.md | Short dated index of significant changes. |
| devlog/README.md | Index of focused case studies and decisions. |
| devlog/ | Separate dated entries for substantial topics. |
| docs/product.md | Current product goals and scope. |
| docs/system-map.md | System relationships and tradeoffs. |
| media/ | Selected screenshots supporting entries. |

The structure follows the needs of this project. Material failures and reversions are recorded when they affect an architectural decision or result.

## Publishing boundary

Game implementation, Unreal assets and rollback history stay private. Reviewed explanations and selected media go to the independent public repository, with traceability retained in the private workshop.

Publication is part of completing relevant development work. A failed push leaves the entry pending; synchronization is reported only after verification.

I use a [repository README](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes) for navigation and adapt the human-readable categories from [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). This is a project-specific documentation design, not a mandatory universal format.
