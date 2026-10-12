# Canadian Fintech Rulebook

A plain-English reference for product managers and designers at Canadian fintechs and banks. Pick the feature you're building and see which regulatory requirements apply, with every requirement linked to the exact section of the official law or regulator guidance.

> **Not legal advice.** These are summaries for product and design teams. Always confirm requirements with your compliance or legal team.

## Status

Early prototype. Feature guides written so far:

- **Marketing messages** (CASL consent, unsubscribe, referral messages; Competition Act misleading messages and drip pricing)
- **Onboarding & KYC** (FINTRAC identity verification, PEP/HIO, third-party determination, account purpose and monitoring; sanctions screening; CRS/FATCA self-certification and SIN; biometric privacy; Bank Act basic banking access)

Planned guides: Payments & transfers, Fees & pricing, Lending & BNPL, Complaints & support, AI & automated decisions, Vendors & cloud, Accounts & deposits, Data & privacy.

## How it works

- **Feature-first:** users start from what they're building, or search for a rule, term or question.
- **Every requirement is cited** to a pinpoint section (e.g. `CASL s.11(3)`) with a link to the official text, labelled as *Law*, *Regulator guidance* or *Best practice*.
- **No user data:** no accounts, cookies or tracking. Checklists live only in the open page.

See [docs/citation-standard.md](docs/citation-standard.md) for the citation rules.

## Project structure

```
content/
  sources.yaml            Registry of official sources (URLs, last-checked dates)
  rules/*.yaml            One structured record per rule
  features/*.md           Feature guides (front matter + Markdown)
docs/
  citation-standard.md    How content must be cited and verified
prototype/
  index.html              Clickable prototype that reads the content files
```

## Run locally

The prototype loads the content files with `fetch`, so it needs a local web server (opening the HTML file directly won't work). From the repository root:

```bash
ruby -run -e httpd . -p 8000
```

Then open http://localhost:8000/prototype/

## Content verification

Items marked `needs_review: true` haven't yet been confirmed against the official source and show a "pending re-verification" label in the UI. Each rule has a `last_verified` date. Found an error? Open an issue with a link to the official source that shows the correct requirement.
