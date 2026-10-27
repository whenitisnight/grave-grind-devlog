# Separating the workshop from the public project library

**27 October 2026 · Repository and documentation architecture**

## Goal

I wanted a portfolio that showed problem-solving as development progressed, while preserving a private workspace for game code, heavy assets and rollback history. Each entry needed to explain the reasoning behind a change and its consequences.

## Repository architecture

I separated the project into two repositories with independent Git histories. The private workshop holds implementation and recovery checkpoints. The public library contains selected documents and gameplay captures.

A concise README and changelog lead to individual dated case studies and stable product and system documents. The development-library index makes entries discoverable without collecting every topic in one long report.

A commit-message trailer links documented private changes to their public entries. A private coverage record handles earlier baseline commits. This provides traceability without publishing private diffs or implementation history.

## Editorial decision

Significant changes, resolved problems, architectural pivots and completed features are documented as they are completed. Related small commits share a case study; routine edits remain in Git history.

I use first person to explain decisions and tradeoffs. Technical sections give the system, behavior or evidence the lead, so ownership stays clear without repeating the same sentence pattern. Each account moves from goal to mechanism and then result, with observed outcomes separated from intentions and unverified claims.

## Verification and limits

Published links, repository visibility and the separation of public content from private implementation were checked. Selected screenshots were reviewed for publication; game assets and raw logs remain private.

This work changes documentation and its workflow. No gameplay change, new build or new gameplay check is claimed. Existing movement evidence retains its original scope and limits. Failed publication remains pending until a successful push is verified.
