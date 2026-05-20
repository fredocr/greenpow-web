# Agent Operating Model

## Purpose

This folder tells coding agents how to work in the GREENPOW web repository over time.

Agents should treat this repository as three different knowledge layers:

1. `PROJECT_BRIEF.md` defines the approved website objective and implementation expectations.
2. `context/` contains approved source-of-truth content for the website.
3. `rnd/` contains exploratory material that can inform future work but is not approved production copy.

## Agent Priorities

When instructions conflict, use this order:

1. Direct user instruction in the current session.
2. `AGENTS.md`.
3. `PROJECT_BRIEF.md`.
4. `agent/` workflow files.
5. `context/` source material.
6. `docs/decisions/` accepted decisions.
7. `rnd/` exploratory notes.

## Working Rules

- Keep English and Spanish pages in parity.
- Add content to `context/` before using it in implementation.
- Promote RND findings into `context/` or `docs/decisions/` before treating them as approved facts.
- Keep form integration centralized.
- Record important structural choices in `docs/decisions/`.
- Record implementation handoffs in `docs/implementation/`.
- Update `agent/evolution-log.md` when agent instructions or repository structure changes.

## Promotion Path

Use this path for uncertain ideas:

```txt
rnd/idea.md
  -> docs/decisions/accepted-decision.md
  -> context/approved-content.md
  -> website implementation
```

Do not skip directly from `rnd/` to production UI unless the user explicitly approves it.
