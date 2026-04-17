---
type: guideline
trigger: When running /evolve-lite:publish and the commit step reports nothing to commit
---

When running evolve-lite publish, check git status in .evolve/public before committing — if working tree is already clean, the entities were published in a prior run and no push is needed.

## Rationale

The publish workflow ran twice with identical output, revealing that re-running publish.py regenerates files but produces no git diff when content is unchanged.
