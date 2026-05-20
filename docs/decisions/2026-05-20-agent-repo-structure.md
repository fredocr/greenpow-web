# Decision: Agent-Ready Repository Structure

Date: 2026-05-20

## Decision

GREENPOW web repository will separate approved content, agent workflow instructions, exploratory research, and implementation documentation into dedicated folders:

```txt
context/
agent/
rnd/
docs/decisions/
docs/implementation/
```

## Rationale

Coding agents such as Replit need clear boundaries between:

- Approved website source material.
- Instructions for how to work in the repository.
- Exploratory research and future ideas.
- Accepted decisions.
- Build handoffs and implementation notes.

Without these boundaries, an agent can accidentally treat research notes as production copy or bury important workflow assumptions in broad project docs.

## Rules

- `context/` is approved content source material.
- `agent/` defines agent operating instructions and build workflow.
- `rnd/` is exploratory and not production truth.
- `docs/decisions/` records accepted decisions.
- `docs/implementation/` records build plans and technical handoffs.

## Consequences

Future agents must promote useful RND findings into `context/` or `docs/decisions/` before using them in public website implementation.
