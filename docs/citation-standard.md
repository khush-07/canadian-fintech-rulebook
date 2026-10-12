# Citation standard

Goal: any reader can check any statement on the site against the official source in one click.

## Rules for writers

1. **Every requirement has at least one citation.** No citation means it can't be published as a requirement.
2. **Cite the exact section (pinpoint)**, e.g. `s.11(3)`, not just "CASL".
3. **Label authority honestly:**
   | Badge | Source type | Meaning to the reader |
   |---|---|---|
   | ⚖️ **Law** | Statute or regulation | Legally binding |
   | 🏛 **Regulator guidance** | Bulletins, guidelines, FAQs | How the regulator interprets the law |
   | 💡 **Best practice** | Our recommendation | Not a legal requirement |
   Best-practice items must never be phrased as "must".
4. **Prefer primary sources.** Use Justice Laws, CanLII, or the regulator's own site, and never law-firm blogs as the citation. Secondary sources can help research but are never shown as the citation.
5. **Paraphrase in plain English and link to the official text.** Federal statute excerpts may be added (permitted under the Reproduction of Federal Law Order), but keep them short.
6. **Track freshness:** `last_checked` per source, `last_verified` per rule. Anything unconfirmed gets `needs_review: true` and shows a ⚠️ "Pending re-verification" label.
7. **Re-verify on a schedule:** every rule at least every 6 months, and immediately when a regulator announces changes.

## How citations appear in the UI

- **Inline superscripts** after each requirement: "Process unsubscribes within 10 business days ¹".
- **Hover / tap popover:** source title, pinpoint, authority badge, "current to" date, and an **Open official text ↗** button that deep-links to the exact section.
- **"Sources" list** at the bottom of every page, generated automatically from the citations.
- **"Copy for PRD"** keeps citations in the copied text, e.g. `(CASL s.11(3))`, so the reference travels into Jira or Figma.
- **"Report an issue"** opens a pre-filled `mailto:` or GitHub issue link. No form submission or data storage on our side.
- A page-level banner: *"Plain-English summary for product teams, not legal advice. Always confirm with your compliance team."*
