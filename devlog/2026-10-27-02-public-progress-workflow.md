# Separating my workshop from my public project library

**27 October 2026 · My project-management decision**

## My goal

I wanted a portfolio that showed how I solved problems as development progressed, while preserving a private workspace for game code, heavy assets and rollback history. I also wanted each entry to explain my reasoning instead of reading like a conversation transcript or a dump of commits.

## My repository architecture

I separated the project into two repositories with independent Git histories. I keep implementation and recovery checkpoints in my private workshop and publish selected documents and gameplay captures in my public library.

I organized the public repository into a concise README, a changelog, individual dated case studies, and stable product and system documents. I use a development-library index to make entries discoverable without turning the portfolio into one long sheet.

I link documented private changes to their public entries through a commit-message trailer and retain a private coverage record for earlier baseline commits. This gives me traceability without publishing private diffs or implementation history.

## My editorial decision

I publish significant changes, resolved problems, architectural pivots and completed features as I finish them. I combine related small commits into the relevant case study and keep routine edits in Git history.

I write each entry in my own first-person voice. I begin with the experience I wanted or the problem I faced, then describe the specific mechanism I chose and why it addresses that problem. I separate observed results from intended outcomes and keep unverified claims explicit.

## My verification and limits

I checked published document links, repository visibility and the separation of public content from private implementation. I reviewed the selected screenshots and kept game assets and raw logs private.

I changed the documentation workflow only; I did not change gameplay or run a new game build for this work. I retain the existing movement evidence with its original scope and limits. I publish documentation alongside relevant development work and record any failed publication as pending.
