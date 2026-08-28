# ProvingGround

A disposable sandbox for exercising the firstmate delivery loop end to end:
hand out a task, run the validation pipeline, open a pull request, merge it,
clean up.

It exists so that loop can be rehearsed for real against a project that does
not matter, instead of against work that does.

## What belongs here

Synthetic content only. Nothing from a real project, nothing private, nothing
that describes anyone's setup. This repository is public and indexed; treat
everything in it as world-readable, because it is.

## What does not belong here

Real project code, operational strategy, worker instructions, credentials,
machine paths, or anything that would be a problem to read aloud.

## The check

`.github/workflows/ci.yml` is deliberately tiny. Its whole job is to give a
pull request a check that can be read as passing or failing, so the "merge
only when green" path has something real to read. It is not a quality gate and
should stay cheap.

## Rehearsal log

- 2026-08-28: worker-runtime rehearsal - Pi harness, Anthropic model, direct-PR loop.
- 2026-08-28: worker-runtime rehearsal - Pi harness, OpenAI model, direct-PR loop.
