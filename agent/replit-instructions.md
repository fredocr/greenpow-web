# Replit Agent Instructions

## Starting Point

Read these files first:

1. `AGENTS.md`
2. `PROJECT_BRIEF.md`
3. `agent/operating-model.md`
4. `agent/build-sequence.md`
5. `agent/content-parity-checklist.md`

Then inspect `context/` for approved content.

## Implementation Expectations

- Use Next.js, TypeScript, Tailwind CSS, and i18n routing unless the user explicitly changes the stack.
- Keep `/en/...` and `/es/...` parity.
- Build reusable product and use-case templates.
- Load strategic content from structured files rather than hardcoding it in components.
- Use one server-side Pipedrive handler for all forms.
- Do not expose Pipedrive secrets to browser code.

## RND Handling

The `rnd/` folder is an idea and research bucket. It is useful context, but it is not production truth.

Before using RND material in website copy, product positioning, legal language, claims, or metadata:

1. Ask whether the finding is approved.
2. Move or summarize it into `context/` or `docs/decisions/`.
3. Use the promoted source in implementation.

## Suggested First Build Task

Scaffold the app shell and route structure first. Do not start by designing individual page visuals. The first useful milestone is a bilingual route tree with shared layout, navigation, content loading, and placeholder pages that prove parity.
