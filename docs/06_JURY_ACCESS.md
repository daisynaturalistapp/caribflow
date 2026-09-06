# Jury Access

This repo is written for a juror who needs the technical argument quickly.

## 60-second path

1. Read [../README.md](../README.md)
2. Read [01_Vision.md](01_Vision.md)
3. Read [02_ARCHITECTURE.md](02_ARCHITECTURE.md)
4. Read [03_SHARED_AND_WITHHELD.md](03_SHARED_AND_WITHHELD.md)
5. Read [04_DATA_SOURCES.md](04_DATA_SOURCES.md)
6. Read [05_DEFECTS_EXCERPTS.md](05_DEFECTS_EXCERPTS.md)

## What to notice

- the system has distinct agent roles
- the model is not the source of truth
- the deterministic layer recomputes the verdict
- publication is human-approved
- unsupported claims are withheld instead of guessed

## What this repo does not try to do

It does not try to prove the whole private codebase.
It tries to prove the parts that matter for judging the project:

- the architecture is real
- the evidence boundary is deliberate
- the refusal behavior is meaningful
- the trade-and-logistics use case is technically grounded
