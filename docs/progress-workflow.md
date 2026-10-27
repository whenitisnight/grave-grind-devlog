# How progress is recorded

Every completed private change set gets a public entry during the same development task. That includes gameplay, art, bug fixes, tests, tooling and documentation. Related commits can share an entry, and small changes can have short entries.

## Entry format

1. **Problem or goal:** what needed to change.
2. **Change:** the resulting behavior or decision, in understandable language.
3. **Evidence:** relevant checks, observed behavior or selected media.
4. **Status and limits:** implemented, verified, pending, reverted or still uncertain.
5. **Next step:** the remaining gap, when relevant.

The changelog indexes entries. Product and architecture documents change when their underlying facts change. Material reversions and unsuccessful outcomes are recorded honestly rather than disappearing from the history.

## Keeping the repositories separate

Game implementation and assets stay private. Public updates are selected summaries and presentation media. No private branches, raw diffs, internal logs or repository history are mirrored here. Internal commit-to-entry traceability is maintained in the private workshop.

Updates are completed alongside development rather than by a timer. If a public push fails, the unpublished entry remains pending and the task reports that gap instead of claiming both repositories are synchronized.

## Conventions

The front page uses a [repository README](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes), and the change index follows the human-readable approach of [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). This is a project workflow, not a claim that GitHub requires one particular portfolio format.
