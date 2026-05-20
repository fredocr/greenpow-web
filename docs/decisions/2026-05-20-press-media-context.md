# Decision: Press And Media Context

Date: 2026-05-20

## Decision

GREENPOW will maintain bilingual press and media source material under:

```txt
context/press/press-media.en.md
context/press/press-media.es.md
```

## Rationale

Press copy needs stricter claim discipline than general marketing copy. Keeping it in `context/press/` gives coding agents a controlled source for press pages, boilerplate, media-contact CTAs, topic lists, and language to avoid.

## Rules

- Use `context/press/` for press and media page content.
- Keep `/en/press` and `/es/prensa` in language parity.
- Route press inquiries through the central Pipedrive form handler with `interest_type=press`.
- Do not publish unverified carbon reduction percentages, certifications, customer names, investor names, partner names, or regulatory claims.

## Consequences

Future press content should be updated in the context files before it is implemented in the website.
