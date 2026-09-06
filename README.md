# CaribFlow

Agentic Regional Opportunity Radar for Caribbean Trade & Logistics

Future Caribbean 2026

Track: Trade & Logistics

Website: https://corridor.trading/

CaribFlow is a governed multi-agent system that helps institutions prioritize trade and logistics
corridors, explain what is blocking activation, and publish only evidence-backed briefs.

This public repository is intentionally curated. It explains the architecture, the evidence
boundary, and the jury-facing proof without publishing the operational scripts, private calibration
values, or real corridor evidence.

## What To Understand

CaribFlow identifies trade and logistics opportunities that are worth activating, then explains:

- what opportunity exists
- why it matters now
- what barriers remain
- what next action would move it forward

The system is built to avoid confident guesswork. Where evidence is missing, it says so. Where a
claim cannot be supported, it is withheld rather than turned into a fake zero.

## Why This Repo Exists

The jury needs enough technical substance to judge the project without seeing the private codebase.
This repo provides that substance in four layers:

1. the agentic architecture
2. the shared vs withheld boundary
3. the public evidence and provenance story
4. a short reading path for jurors

## Start Here

1. Read [docs/01_Vision.md](docs/01_Vision.md)
2. Read [docs/02_ARCHITECTURE.md](docs/02_ARCHITECTURE.md)
3. Read [docs/03_SHARED_AND_WITHHELD.md](docs/03_SHARED_AND_WITHHELD.md)
4. Read [docs/04_DATA_SOURCES.md](docs/04_DATA_SOURCES.md)
5. Read [docs/05_DEFECTS_EXCERPTS.md](docs/05_DEFECTS_EXCERPTS.md)
6. Read [docs/06_JURY_ACCESS.md](docs/06_JURY_ACCESS.md)

## What Is Deliberately Not Published

- operational scripts and orchestration plumbing
- private calibration values
- real corridor evidence and archived snapshots
- agent prompt text and configuration
- git history
- machine names, tokens, personal paths, and internal-only identifiers

## Why This Is Agentic

CaribFlow divides the work across distinct roles with distinct responsibilities, outputs, and
stop conditions. Evidence is gathered, structured, verified, and only then considered for
publication.

The handoff between roles is explicit. Verification is separated from generation, and the system
can refuse to publish when the evidence is not sufficient.

## Why It Fits The Buildathon

The buildathon asks for more than a chatbot demo. CaribFlow shows a working multi-agent workflow
for trade and logistics that includes:

- role-based delegation
- deterministic verification
- traceable evidence use
- human review before publication
- applied value in corridor prioritization and activation

That is the system being demonstrated, not a story added on top of it.

## Why Local Inference Works Here

CaribFlow uses local inference with open-source models because the system is split between
judgment and verification.

The agentic layer handles interpretation and drafting. The deterministic layer handles scoring,
gating, and publication rules. That separation makes local inference practical: the model does not
need to be the system of record, only a bounded part of the workflow.

That choice is deliberate:

- it keeps operating cost under control
- it reduces energy and network overhead
- it avoids sending sensitive working context to a third-party service
- it makes the system easier to reproduce and audit on constrained infrastructure

For this project, the point is not bigger models. The point is a disciplined setup where the model
is one part of a bounded workflow, and the code keeps the outputs grounded.

## Public Repo Contents

- `docs/` for architecture, evidence boundaries, security, and jury access
- `LICENSE` for the public distribution terms
- `assets/brand-mark.svg` for the public site icon
