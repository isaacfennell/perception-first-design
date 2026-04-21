---
id: l017
title: "Iterative Analysis Regression Is Deeper Visibility, Not Failure"
layer: meta
date: 2026-03-10
contributor: Stefan Kovalik
related: [l006]
tags:
  - iterative-analysis
  - regression
  - impasse
  - forge
  - ralph-loop
source: PFD RL practitioner workflow across 10+ Forge sessions (Cognograph plans, design systems, resumes, book chapters)
---

# Learning 17: Iterative Analysis Regression Is Deeper Visibility, Not Failure

**Insight:** When an iterative PFD analysis (multi-round "Forge" loop) shows a score DROP around rounds 3-6, the cause is almost never that fixes made things worse. The cause is that resolving surface-level issues (nav overload, font proliferation) unmasks deeper problems that were previously invisible — the dominant signal was drowning out subtler violations. The regression reflects updated understanding, not degraded quality. The correct framing is "with the obvious issues resolved, the analysis can now see problems that were previously masked." This is analogous to Learning #6 (Infrastructure ≠ Activation) — the deeper issues existed all along, but the perceptual infrastructure to detect them only activated once the surface was cleared. **Practical implication:** Iterative analysis tools must frame regression pragmatically ("found something, score dropped, here's the cause, apply fix?"), not as failure. If regression persists across 2+ consecutive rounds, the artifact may need a fundamentally different approach — that's an impasse, not a bug. Three terminal states for iterative analysis: converged (done), impasse (can't converge with current premise), abandoned (user stopped). The impasse state is the missing piece in most iterative tooling — tools either converge or give up, but the middle state where the tool says "this approach won't get you there" is the highest-value signal.
