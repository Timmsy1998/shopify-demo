# Atelier Theme

Shopify theme repo for the Atelier dev store.

Started from Dawn so we have a stable base, then we layer Atelier-specific sections/styles on top.

## Requirements

- Node 20+
- npm 10+
- Shopify dev store access

## Setup

```bash
cp .env.example .env
npm install
```

Add store values in `.env`:

- `SHOPIFY_STORE=your-store.myshopify.com`
- `SHOPIFY_THEME_ID=123456789` (optional until you pick a target theme)

## Daily commands

```bash
npm run dev
```

Starts local theme dev against `SHOPIFY_STORE`.

```bash
npm run list
```

Lists themes in the store.

```bash
npm run pull
npm run push
```

Pull/push against `SHOPIFY_THEME_ID`.

```bash
npm run check
```

Runs Theme Check.

## Notes

- `.env` is local-only and gitignored.
- Keep Dawn core patterns where useful; build Atelier-specific features in separate commits.
