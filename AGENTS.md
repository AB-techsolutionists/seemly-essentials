# Seemly Essentials — Shopify Theme Customization

## Overview
Customize a merchant Shopify theme using Shopify CLI + local theme files.

## Auth
- Use Shopify CLI session (`shopify theme pull --store <store>`).
- Do NOT hardcode `.myshopify.com` admin tokens in repo files.

## Workflow
1. Pull theme code: `shopify theme pull --store <store>`
2. Edit locally: Liquid, CSS, JS, JSON.
3. Preview: `shopify theme dev` → http://127.0.0.1:9292
4. Push: `shopify theme push` (or `--unpublished` for a new theme)
5. Publish: `shopify theme publish`

## Rules
- Keep changes minimal and merchant-safe.
- Do not run destructive or irreversible actions without confirming.
- Theme files are store-specific; keep secrets out of this repo.
