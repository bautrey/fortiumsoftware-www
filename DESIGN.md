# Fortium Software Marketing Site Design

**Date**: 2026-01-31
**Status**: Approved

## Overview

A static "coming soon" teaser site for Fortium Software's platform at `www.fortiumsoftware.com`. Explains what Fortium does today (LaaS operations via Engage) and hints at the future (Execute / Leadership Execution Platform).

## Pages

| Path | Purpose |
|------|---------|
| `/` | Home — Hero, platform story, links to Engage & Execute |
| `/engage` | Engage product page — LaaS operational tools |
| `/execute` | Execute product page — "Coming Soon" teaser for LXP |

## Tech Stack

- Static HTML + Tailwind CSS
- No server, no framework
- Deploy to Render static site
- Same Fortium branding as Engage/Identity (blue shield, clean typography)

## Project Structure

```
fortium-www/
├── index.html          # Home
├── engage/index.html   # Engage product page
├── execute/index.html  # Execute coming soon
├── css/
│   ├── input.css       # Tailwind directives
│   └── styles.css      # Built output
├── images/
│   └── fortium-logo.svg
├── tailwind.config.js
├── package.json
└── render.yaml
```

## Page Designs

### Home (`/`)

**Hero**:
- Fortium shield logo (prominent)
- Headline: "The Operating System for Leadership as a Service"
- Subhead: "We built the tools that power world-class executive leadership. Now we're making them available to everyone."

**Platform Cards** (2-up):
- **Engage** — "The operational backbone for Leadership as a Service" → `/engage`
- **Execute** — "The Leadership Execution Platform" (Coming Soon) → `/execute`

**Footer**:
- © 2026 Fortium Software
- Employee login link → `https://identity.fortiumsoftware.com`

### Engage (`/engage`)

**Hero**:
- "Engage" headline
- Subhead: "The operational backbone for Leadership as a Service"
- CTA: "Sign in to Engage" → `https://engage.fortiumsoftware.com`

**Applications Grid** (8 apps, no groupings):
| App | Description |
|-----|-------------|
| Identity | Centralized authentication and access control |
| Talent | Talent management and operations |
| Pipeline | Deal flow and pipeline analytics |
| Gateway | Candidate portal and onboarding |
| Outbound | Signal-based outreach workflow |
| Payouts | Partner payment processing |
| Atlas | Profile enrichment and data |
| Ideas | Feature requests and roadmap |

### Execute (`/execute`)

**Coming Soon**:
- "Execute" headline
- Subhead: "The Leadership Execution Platform"
- Teaser: "A new way for organizations to access world-class executive leadership. Coming soon."
- No email capture for now — just a clean teaser

## Deployment

- Render static site: `www.fortiumsoftware.com`
- DNS: CNAME `www` → Render static site URL
- Redirect root `fortiumsoftware.com` → `www.fortiumsoftware.com` (or vice versa)

## Design Principles

- Professional, confident, understated
- Not salesy — "here's what we're building"
- Clean, minimal, fast-loading
- Consistent with Engage/Identity branding
