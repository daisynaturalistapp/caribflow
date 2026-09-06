# Shared and Withheld

The rule is simple:

> The mechanism is the claim; the numbers behind it are the asset.

This public repo shares the mechanism.
It withholds the asset.

## Shared

- the architecture
- the jury access path
- the public source families
- the security posture
- curated defect excerpts
- the existence of evidence and provenance controls
- the public calibration shape, if published separately as a placeholder-only file

## Withheld

- private calibration values
- real evidence corpora
- real corridor snapshots
- agent prompt text
- orchestration plumbing tied to providers
- git history
- internal-only identifiers, machine names, tokens, personal paths
- any code that would let the reader reconstruct the hidden judgement layer

## Why this boundary exists

Publishing the wrong layer would not make the project more transparent.
It would make the judgement easier to copy without the corresponding discipline.

The public repo therefore explains how the system works without giving away the full operating
surface that makes it valuable.

## What the jury can still learn

- how the agents divide the work
- how the deterministic layer constrains the model
- how the publication gate protects the output
- how evidence provenance is preserved
- why the system is suitable for institutional trade and logistics use

## What the jury should not need

The jury should not need the private code to understand the claim.
It should need the private code only if it were trying to reproduce the full internal asset,
which is not the purpose of the public repository.
