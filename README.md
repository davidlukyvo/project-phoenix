# Project PHOENIX

Public professional portfolio for Vo Thanh Sang.

## Publishing model
- Static HTML/CSS
- GitHub repository as source of truth
- Cloudflare Pages for hosting
- Later: custom domain

## Privacy guardrail
Never publish:
- internal IP addresses / hostnames
- credentials, tokens, tenant IDs or app secrets
- confidential company metrics
- proprietary diagrams/configurations
- personal or customer data

## Daily article workflow
A new article should:
1. be grounded in a confirmed career/project theme,
2. generalize company-specific implementation details,
3. emphasize engineering reasoning and lessons learned,
4. avoid claims that cannot be verified,
5. update `blog/index.html` and the Latest Writing section on `index.html`.

## Cloudflare Pages
Once the GitHub repository is public:
1. Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git.
2. Select the repository.
3. Framework preset: None.
4. Build command: leave blank.
5. Build output directory: `/`.
6. Deploy.
