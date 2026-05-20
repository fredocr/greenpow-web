# GREENPOW Web Agent Instructions

Use this repository to build a bilingual GREENPOW website.

## Non-Negotiable Requirements

- Build every public page in English and Spanish.
- Use `/en/...` and `/es/...` route prefixes.
- Never create an English route without a Spanish route with matching layout, metadata, CTA structure, and form behavior.
- Use structured content from `context/` as the source of truth.
- Do not hardcode strategic positioning, product copy, legal copy, or vertical copy directly inside components.
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

The context files are implementation inputs. If a page needs copy, metadata, CTA text, FAQs, product descriptions, legal content, or form requirements, read from `context/` first and keep language parity.

## Design Direction

The site should feel like modern infrastructure software: precise, credible, technical, calm, and commercial. Avoid a generic hosting-company feel. Avoid one-off page layouts when a product or vertical template can serve the same purpose.
