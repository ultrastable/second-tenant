# AGENTS.md

The protocol for every agent in this repo is in [`agents/AGENTS.md`](agents/AGENTS.md). Read it first, then your role file in [`agents/roles/`](agents/roles/). Limits: [`autonomy/policy.json`](autonomy/policy.json).

## Build and test

Run these from the repository root before you open a pull request.

- `python3 -m unittest discover -s tests`: the Python tests.
- `cd worker && npm test`: the Worker's tests.
- `python3 scripts/check_readmes.py`: the READMEs agree with the code.

## Rules

- Every standing rule in full, including the axioms (closed loop, boundary, agent consumption, terms, code-only order): [`agents/AGENTS.md`](agents/AGENTS.md).
- Hard limits: never print or commit a secret; do not weaken a check to make it pass; the only pause is the interrupt gate described there.
