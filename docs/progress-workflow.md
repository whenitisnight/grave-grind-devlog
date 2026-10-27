# How I document progress

I want this portfolio to explain my decisions and their consequences. I publish when I reach a major milestone, resolve a meaningful problem, make a significant architectural pivot or complete a feature. I also make an entry whenever I explicitly choose to log a piece of work for the public repository.

I group related commits into the relevant entry and keep routine edits in Git history. I maintain the library continuously as substantial work is completed.

## My writing format

I start with the goal I wanted to achieve or the problem I faced. I then explain the actual technical mechanism I chose, why it addresses the problem, the evidence I have and the remaining limits.

I write in the first person and use direct, professional language. I describe my architectural decisions without retelling conversations. I tie technical claims to changes that actually happened and distinguish plans from implemented behavior.

## My library structure

| Location | How I use it |
| --- | --- |
| README.md | I introduce the project, current status and navigation. |
| CHANGELOG.md | I keep a short dated index of significant changes. |
| devlog/README.md | I index focused case studies and decisions. |
| devlog/ | I give each substantial topic its own dated entry. |
| docs/product.md | I maintain my current product goals and scope. |
| docs/system-map.md | I explain my system relationships and tradeoffs. |
| media/ | I retain selected screenshots that support an entry. |

I adapt this structure to the project instead of forcing every topic into one report. I record material failures and reversions when they affect an architectural decision or result.

## My publishing boundary

I keep game implementation, Unreal assets and rollback history private. I publish reviewed explanations and selected media in the separate public repository and retain traceability to the relevant private work.

I publish as part of completing relevant development work. If a public push fails, I retain the entry as pending rather than claiming both repositories are synchronized.

I use a [repository README](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes) for navigation and adapt the human-readable categories from [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). I treat this as my project’s documentation design rather than a mandatory universal format.
