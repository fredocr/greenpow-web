# GREENPOW Web Agent Instructions

Use this repository to build a bilingual GREENPOW website.

## First Files To Read

1. `PROJECT_BRIEF.md`
2. `agent/operating-model.md`
3. `agent/build-sequence.md`
4. `agent/content-parity-checklist.md`
5. `agent/marketing-content-rules.md` when writing copy
6. `agent/replit-instructions.md` when working in Replit

## Non-Negotiable Requirements

- Build every public page in English and Spanish.
- Use `/en/...` and `/es/...` route prefixes.
- Never create an English route without a Spanish route with matching layout, metadata, CTA structure, and form behavior.
- Use structured content from `context/` as the source of truth.
- Use `context/marketing/`, `context/audiences/`, `context/regions/`, `context/claims/`, `context/seo/`, `context/campaigns/`, `context/website/`, `context/design/`, and `context/components/` when generating marketing pages, campaign pages, SEO content, or component copy.
- Use `agent/marketing-content-rules.md` when generating copy.
- Do not hardcode strategic positioning, product copy, legal copy, press copy, or vertical copy directly inside components.
- Present GREENPOW as product-led infrastructure technology, not only managed hosting or services.
- Keep the mission clear: reduce the carbon footprint of cloud computing.
- Explain MySx as the algorithmic layer for moving compute based on carbon intensity, energy price, infrastructure availability, cost, and performance signals.
- Explain Cortex as organizational memory for autonomous agents.
- Connect all public forms through one central Pipedrive form handler.
- Preserve legal page routes for privacy, cookies, and terms in both languages.

## Suggested Stack

- Next.js
- TypeScript
- Tailwind CSS
- MDX or structured content files
- i18n routing
- Server-side form endpoint for Pipedrive integration

## Content Ownership

The context files are implementation inputs. If a page needs copy, metadata, CTA text, FAQs, product descriptions, legal content, press content, campaign copy, visual guidance, claim policy, persona messaging, regional positioning, or form requirements, read from `context/` first and keep language parity.

## Source Priority

When sources disagree, use this order:

1. Direct user instruction in the current session.
2. This `AGENTS.md` file.
3. `PROJECT_BRIEF.md`.
4. Files in `agent/`.
5. Approved source material in `context/`.
6. Accepted decisions in `docs/decisions/`.
7. Research notes in `rnd/`.

## RND Bucket Rule

The `rnd/` folder exists for research, hypotheses, experiments, and future ideas. Agents may read it for context, but must not treat it as approved production copy, product commitment, legal language, metadata, or impact evidence.

Before using an RND idea publicly, promote the accepted conclusion into `context/`, `PROJECT_BRIEF.md`, or `docs/decisions/`.

## Design Direction

The site should feel like modern infrastructure software: precise, credible, technical, calm, and commercial. Avoid a generic hosting-company feel. Avoid one-off page layouts when a product or vertical template can serve the same purpose.
