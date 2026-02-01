# Fortium Software Marketing Website

> Public marketing site for Fortium Software platform
> Target URL: https://www.fortiumsoftware.com

## Overview

Static marketing site introducing Fortium Software's platform. Currently a "coming soon" teaser with:
- **Home** (`/`) - Platform overview, links to Engage and Execute
- **Engage** (`/engage`) - LaaS operational tools (live today)
- **Execute** (`/execute`) - Leadership Execution Platform (coming soon)

## Tech Stack

- **Static HTML** + Tailwind CSS
- **No server** - pure static files
- **Deployment**: Render static site (planned)

## Project Structure

```
.
├── index.html           # Home page
├── engage/index.html    # Engage product page
├── execute/index.html   # Execute coming soon page
├── css/
│   ├── input.css        # Tailwind directives
│   └── styles.css       # Built output (gitignored)
├── images/              # Logo, favicon
├── tailwind.config.js
├── package.json
└── render.yaml          # Render static site config
```

## Development

### Build CSS
```bash
npm install
npm run build:css    # One-time build
npm run dev          # Watch mode
```

### Preview locally
```bash
npx serve .
# Open http://localhost:3000
```

## Content

### Engage Page Apps (8 total)
- Identity - Centralized authentication and access control
- Talent - Talent management and operations
- Pipeline - Deal flow and pipeline analytics
- Gateway - Candidate portal and onboarding
- Outbound - Signal-based outreach workflow
- Payouts - Partner payment processing
- Atlas - Profile enrichment and data
- Ideas - Feature requests and roadmap

### Execute Page
Coming soon teaser for the Leadership Execution Platform (LXP / Seat OS vision).

## Deployment (Not Yet Deployed)

Planned:
1. Create Render static site
2. Configure custom domain `www.fortiumsoftware.com`
3. Set up redirect from `fortiumsoftware.com` → `www.fortiumsoftware.com`

## Related Projects

- **Engage app** (`../engage`) - The actual Engage application at engage.fortiumsoftware.com
- **Identity** (`../identity`) - OIDC provider at identity.fortiumsoftware.com
- **LxP** (`../lxp`) - Leadership Execution Platform (referenced in Execute page)

## Design Reference

See `DESIGN.md` for the full design spec from brainstorming session.

## Repository

- **GitHub**: `bautrey/fortiumsoftware-www` (private, personal account)
- Separate from FortiumPartners org since this is Fortium Software branding
