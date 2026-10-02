# CLAUDE.md — DailyVaults Shopify theme

This repo is a Shopify Online Store 2.0 theme (Liquid, JSON templates, sections, blocks).

## Layout
- `layout/` theme.liquid wrapper
- `templates/` JSON templates (product, collection, index, ...)
- `sections/`, `blocks/`, `snippets/` reusable Liquid
- `assets/` CSS/JS/images
- `config/settings_schema.json` theme settings; `config/settings_data.json` is store-edited, avoid hand edits
- `locales/` translation strings

## Workflow
- Preview: `shopify theme dev --store fk0p3v-vs.myshopify.com`
- Lint: `shopify theme check`
- Never `shopify theme push` to the live/published theme without asking; use `--unpublished` or a dev theme.
- Work on a branch and open a PR; `main` may be synced to the store via Shopify's GitHub integration.

## Conventions
- Keep sections schema-driven so merchants can edit in the theme editor.
- Mobile-first CSS; check pages at 375px width.
- No hard-coded prices, currency, or product IDs — use Liquid objects.
