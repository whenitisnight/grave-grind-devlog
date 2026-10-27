# Public development journal

This repository is the public portfolio and ongoing progress log for Grave / Grind. The game implementation lives in a separate private workshop.

- Every completed private change set needs a corresponding public entry, including gameplay, fixes, art, testing, tooling and documentation. Related commits may share an entry; do not defer small changes until a major milestone.
- Update `CHANGELOG.md` and add or update a dated entry under `devlog/`. Record the problem, change, evidence, status and remaining work. Use brief entries for small changes.
- Update the README, product brief and system map when the underlying facts change. A publishing-only typo correction can be a small public documentation commit.
- Publish updates as part of completing development work. This is an event-driven workflow, not an unattended background timer.
- Inspect branch and working-tree state first. Preserve unrelated edits. Use focused commits and push completed public updates. For ordinary additive journal entries, direct commits to this repository's `main` are allowed; larger public-document restructures can use pull requests.
- Only publish deliberately reviewed documents and selected game media. Never mirror the private repository, private branches or history. Never copy raw source, Unreal assets, build outputs, internal logs, credentials or machine paths here. Preserve the explicit `.gitignore` allowlist.
- Be accurate about prototypes, AI-assisted development, automated input replays, rendered-frame review, hands-on play and unverified goals. Do not present planned features as completed or test counts as proof of game quality.
- The public log needs useful explanations, not private commit messages or diffs copied verbatim. Internal traceability belongs in the private repository.
