# DailyVaults Store

Shopify theme for the DailyVaults store, set up for editing with Claude Code.

## Setup

```bash
npm install -g @shopify/cli
shopify theme pull --store fk0p3v-vs.myshopify.com   # pull the live theme into this repo
shopify theme dev  --store fk0p3v-vs.myshopify.com   # local preview with hot reload
shopify theme push --unpublished                        # push changes as a new draft theme
```

Optional: in Shopify admin → Online Store → Themes → Add theme → Connect from GitHub, pick this repo's `main` branch so commits sync to the store automatically.
