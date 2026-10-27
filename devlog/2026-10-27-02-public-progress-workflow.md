# Making progress visible as development happens

**27 October 2026 · Development workflow**

## Goal

Maintain a public portfolio that shows how the project evolves while keeping the game implementation and heavy assets in a private workshop.

## Change

A dedicated public journal now holds a project overview, product brief, conceptual system map, dated development entries and selected game captures. The private repository retains implementation history and rollback checkpoints.

The publishing rule applies to **every completed private change set**, including small fixes, tests, tooling and documentation. Related commits can share a concise entry. The public log is maintained during development rather than postponed until a major milestone or a future portfolio launch.

Private commits link to their public entry through a commit-message trailer. Older baseline commits have a private coverage record. Public entries describe the work without publishing private commit messages, raw diffs or source history.

## Evidence and limits

This update changes the development and documentation workflow. It does not change gameplay or require a new game build. The movement results referenced elsewhere in this journal are the previously verified checkpoint.

The ongoing responsibility is to keep both repositories current as each task is completed, and to report any publication failure explicitly. This workflow is part of development work; it is not an unattended background service.
