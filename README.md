# Project PHOENIX

Public professional portfolio for Vo Thanh Sang.

## Architecture
- `public/` — the only directory published to the web
- `public/blog/` — engineering notes
- `public/assets/` — CSS, favicon and social assets
- `public/data/career.json` — public-safe career data
- `wrangler.jsonc` — Cloudflare Workers Static Assets configuration

## Deployment
GitHub is the source of truth. Cloudflare Workers Builds runs `npx wrangler deploy`; Wrangler publishes only `./public`.

Current development URL: `project-phoenix.davidlukyvo.workers.dev`

## Privacy guardrail
Never publish:
- internal IP addresses or hostnames
- credentials, tokens, tenant IDs or app secrets
- confidential company metrics
- proprietary diagrams/configurations
- personal, employee or customer data

## Article workflow
Every article must:
1. be grounded in a confirmed career/project theme,
2. generalize company-specific implementation details,
3. emphasize engineering reasoning and lessons learned,
4. avoid unsupported claims,
5. pass the privacy guardrail before publication,
6. update the writing index, homepage Latest Writing section and sitemap.

## Future custom domain
When a custom domain is added, update the canonical URL, Open Graph URL, `robots.txt` and `sitemap.xml` from the workers.dev hostname to the final domain.
