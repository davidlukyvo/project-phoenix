# Project PHOENIX

Public professional portfolio for Vo Thanh Sang.

## Architecture
- `public/` — the only directory published to the web
- `public/blog/` — engineering notes
- `public/assets/` — CSS, favicon and social assets
- `public/data/career.json` — public-safe career data
- `EDITORIAL_STYLE.md` — writing voice and publishing tone for the whole site
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
2. follow the voice in `EDITORIAL_STYLE.md`: practical, specific, reflective and not inflated,
3. generalize company-specific implementation details where needed for privacy,
4. show engineering reasoning through real decisions, validation, trade-offs and lessons learned,
5. avoid unsupported claims and unnecessary corporate/brochure language,
6. pass the privacy guardrail before publication,
7. update the writing index, homepage Latest Writing section and sitemap when appropriate.

The site should feel like field notes from someone who has worked in Infrastructure for many years — not a consulting brochure and not a collection of slogans.

## Future custom domain
When a custom domain is added, update the canonical URL, Open Graph URL, `robots.txt` and `sitemap.xml` from the workers.dev hostname to the final domain.
