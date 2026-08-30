# Project agent memory

ProvingGround is a disposable, public sandbox for rehearsing the delivery loop
end to end — task, validation, pull request, merge, cleanup — against a project
that does not matter. See `README.md` for what it is and why it exists.

## The rule that outranks everything else

**Synthetic content only.** This repository is public and world-readable, so
everything committed here must be safe to read aloud: no real project code, no
operational strategy, no worker instructions, no credentials, no machine paths.
Read README's "What belongs here" and "What does not belong here" before adding
anything, and hold every file — this one included — to that bar.

## The check

`.github/workflows/ci.yml` is deliberately tiny. It exists only so a pull
request carries a check that reads as passing or failing, giving the
merge-when-green path something real to read. It is not a quality gate; keep it
cheap.

## Maintaining this file

Keep this file for knowledge useful to almost every future agent session in this project.
Do not repeat what the codebase already shows; point to the authoritative file or command instead.
Prefer rewriting or pruning existing entries over appending new ones.
When updating this file, preserve this bar for all agents and keep entries concise.
