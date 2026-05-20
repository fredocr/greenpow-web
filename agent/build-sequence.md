# Build Sequence

## Phase 1: Foundation

- Confirm package manager and runtime.
- Scaffold Next.js, TypeScript, Tailwind CSS, and i18n routing.
- Create `/en/...` and `/es/...` route groups.
- Add content loading from structured files or MDX.
- Add shared layout, navigation, footer, SEO metadata, and language switcher.

## Phase 2: Content System

- Convert approved `context/` documents into structured page data.
- Create reusable templates for products and use cases.
- Add language parity checks.
- Keep strategic copy outside React components.

## Phase 3: Core Pages

- Build homepage.
- Build technology page.
- Build products index and product detail pages.
- Build use-cases index and vertical pages.
- Build impact, partners, funding, about, and contact pages.
- Build legal pages.

## Phase 4: Forms And CRM

- Build shared form components.
- Build one server-side Pipedrive handler.
- Add hidden tracking fields for source page and UTM parameters.
- Add localized success and error states.
- Keep Pipedrive secrets server-side.

## Phase 5: Quality Gates

- Validate route parity.
- Validate content source mapping.
- Validate responsive layout.
- Validate form behavior.
- Validate SEO metadata in both languages.
- Run lint, typecheck, and build.

## Phase 6: Evolution

- Move approved research from `rnd/` into `context/` or `docs/decisions/`.
- Add new routes through reusable templates.
- Update agent docs when workflow assumptions change.
