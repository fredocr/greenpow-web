# Agent Structure Design

Date: 2026-05-20

## Goal

Improve the GREENPOW web repository so coding agents such as Replit can understand the project, evolve it safely over time, and separate approved content from exploratory research.

## Current State

The repository already contains:

- `PROJECT_BRIEF.md`
- `AGENTS.md`
- `README.md`
- `context/` with bilingual brand, product, sales, funding, impact, partner, legal, forms, and vertical material.

There is no RND bucket before this change.

## Approved Structure

Add:

```txt
agent/
rnd/
docs/decisions/
docs/implementation/
docs/superpowers/specs/
docs/superpowers/plans/
```

## Responsibilities

`agent/` contains workflow instructions for coding agents.

`rnd/` contains exploratory research, hypotheses, experiments, competitor notes, roadmap ideas, and product research.

`docs/decisions/` records accepted decisions.

`docs/implementation/` records handoffs and implementation notes.

`docs/superpowers/` records Superpowers specs and plans.

## RND Rule

RND content is useful context, but it is not approved production truth. Agents may read it, but must promote accepted ideas into `context/`, `PROJECT_BRIEF.md`, or `docs/decisions/` before using them in public website copy, metadata, claims, or implementation commitments.

## Success Criteria

- Replit and other coding agents have a clear starting path.
- RND exists and has guardrails.
- Future repository evolution has a place to be recorded.
- The existing bilingual context model remains intact.
