# Curated Defect Excerpts

This file includes a small number of representative defects, not the full raw register.
The point is to show engineering discipline without dumping the entire issue log.

## 1. Evidence-grounding defect

- Problem: a route could be credited from a source that did not actually attest both corridor ports.
- Why it matters: a false positive at the evidence layer weakens the entire brief.
- What it proved: the system must only count a route when the source truly supports it.
- Why the jury should care: this is the opposite of a hallucinated claim.

## 2. Duplicate-gate defect

- Problem: a duplicated export or publication filter existed in a way that could send readers to the
  wrong canonical path.
- Why it matters: if the wrong copy becomes the reference, the public story can diverge from the
  enforced story.
- What it proved: the public path must have one canonical gate and one canonical explanation.
- Why the jury should care: engineering maturity is not only about features; it is about not
  letting two definitions of the same rule drift apart.

## 3. Publication-wording defect

- Problem: model-written wording sometimes described a score as if it were something else.
- Why it matters: a correct score paired with a misleading explanation is still a bad output.
- What it proved: the publication layer must check that the wording matches the evidence held.
- Why the jury should care: this is the core agentic discipline of the project.

## What these excerpts demonstrate

- the system can refuse bad evidence
- the system can correct itself under guard
- the system does not rely on prose alone
- the public story is anchored in actual engineering failures, not only in aspiration
