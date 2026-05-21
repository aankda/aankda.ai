# AANKDA-HUB

Public website repository for [aankda.ai](https://aankda.ai), including the brand site, product catalog, product landing pages, and public policy surfaces for AANKDA LLC.

## Overview

This repository is the public web layer for AANKDA. It is responsible for outward-facing product messaging, support and privacy surfaces, shared brand assets, and static-site metadata.

Public copy in this repository should remain aligned with the actual state of the corresponding product repositories. This repository is the publishing layer, not the authoritative source for every product behavior claim.

## Repository Scope

- Brand homepage and company context
- Product catalog and product-specific landing pages
- Support, privacy, terms, and related policy surfaces
- Shared styles, scripts, fonts, icons, and metadata
- Static-site validation and publishing support files

## Project Structure

- `index.html`, `about/`, `products/`: brand-level entry points
- product route directories: product-specific public pages and assets
- `assets/`: shared brand assets, fonts, scripts, and styles
- `templates/`: reusable public-page templates
- `scripts/`: validation and maintenance scripts
- `.github/workflows/`: repository automation and contract checks

## Validation

Before publishing public-shell or metadata changes, run:

```bash
node scripts/validate-public-contract.mjs
```

This check verifies shared page-contract requirements such as metadata, canonical links, header structure, and theme-controller wiring.

## Deployment

The site is published via GitHub Pages from the repository's `main` branch.

## Change Guidelines

- Keep messaging specific, calm, and release-stage accurate.
- Avoid product claims that are not supported by the current companion product repository.
- Prefer updating shared assets and shared shell structures consistently rather than patching individual pages ad hoc.
- Treat support, privacy, and legal wording as user-facing contract surfaces and update them carefully.

## Contact

- Support: `support@aankda.ai`
- Privacy: `privacy@aankda.ai`
- Legal: `legal@aankda.ai`

## License

See [LICENSE](LICENSE).
