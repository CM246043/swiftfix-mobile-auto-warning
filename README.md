# Swift Fix Mobile Auto Warning

Live site: https://cm246043.github.io/swiftfix-mobile-auto-warning/

A small, static public-information website designed to clearly present a consumer warning tied to a business name and its public-record trail. The project is intentionally simple, transparent, and easy to audit: no backend, no user accounts, no hidden processing, and no database.

## Purpose

This site exists to help consumers evaluate risk before paying for mobile auto repair services by organizing public-facing evidence into a readable, searchable format. The focus is not to make accusations without basis; it is to make the underlying public-record trail easier to review.

## User and primary goal

- User: consumers, researchers, and concerned parties evaluating a business before hiring it
- Goal: provide a clear, referenceable summary of public records and business continuity so readers can assess warning signals before entering a transaction
- Desired outcome: a website that is easy to understand, easy to verify, and easy to maintain without complex tooling

## Core workflow

1. Research business identity and ownership trail
2. Collect public-record references from court, business filings, complaint history, and reputation profiles
3. Confirm alternate business names and continuity of ownership
4. Organize findings into a timeline and evidence archive
5. Publish a static HTML site with links to source material and supporting screenshots
6. Keep the information auditable by clearly labeling sources and dates

## Data used

This project relies on publicly available information and archived screenshots, including:

- Arizona Corporation Commission business entity records
- Better Business Bureau public profiles and historical screenshots
- Public court and municipal records references
- Police and sheriff record references tied to the same owner or business name
- Archived public screenshots used as evidence of historical display states

Important note: This project is informational only and should not be treated as legal advice or a definitive finding of wrongdoing. It is a record-keeping and consumer-alert page based on public information.

## Minimum viable product (MVP)

The MVP is intentionally modest and effective:

- A home page with a warning summary and business overview
- A public-record timeline page
- A business connection page explaining ownership continuity across alternate names
- An evidence index linking to screenshots and supporting references
- Clear disclosure that the site is based on public records and requires independent verification

This approach keeps the project low-cost, transparent, and easy to update without unnecessary complexity.

## Architecture

This repository uses a simple static-site architecture:

- HTML pages in the root directory
- CSS embedded directly in each page for minimal dependency overhead
- Local image assets stored in the repository for evidence and record screenshots
- GitHub Pages for publishing from the main branch
- No backend, no package manager, no build pipeline, no database, and no user data collection

Recommended design principles:

- Keep content readable and text-first
- Use stable filenames for evidence assets
- Maintain direct links to conservative public sources
- Separate main narrative pages from evidence pages to improve auditability
- Prefer clear, dated source notes over complicated interactivity

## Privacy and risk considerations

Because the project deals with public records and personal business associations, privacy and risk should be handled carefully.

Key considerations:

- Use only information already in the public record or publicly archived
- Avoid adding private or non-public details not essential to the consumer warning
- Clearly distinguish between a business warning, a public record summary, and legal conclusions
- Label the site as informational and not a legal determination
- Be cautious about including sensitive personal information beyond what is necessary for consumer context
- Maintain source references for every material claim

This is a consumer-information project, not a data-collection platform. The default should be minimal exposure, maximum transparency, and conservative sourcing.

## Implementation sequence

1. Define the scope and audience
   - Consumer warning / public records summary
   - Clear audience and objective
2. Gather and verify sources
   - Confirm business names, ownership trail, and public-record references
   - Preserve source links and archive screenshots when available
3. Create the static site structure
   - Home page
   - Timeline page
   - Case/ownership page
   - Evidence index
4. Add narrative and evidence content
   - Business overview
   - Public record summary
   - Verification instructions for readers
   - Dated screenshots with captions
5. Validate the site locally
   - Open HTML pages in a browser
   - Confirm links resolve correctly
   - Confirm image paths work and pages render as expected
6. Configure GitHub Pages
   - Ensure the repository is public or whichever visibility is desired
   - Enable GitHub Pages from the main branch
   - Confirm the site loads at the published URL
7. Review for risk and clarity
   - Check claims against source material
   - Remove unsupported or unclear statements
   - Improve wording to be factual and balanced
8. Publish and maintain
   - Keep evidence archive current when new public records emerge
   - Document revisions and update dates clearly

## Local development and verification

Because this is a simple static website, local use is straightforward:

1. Clone the repository
2. Open the HTML files in a browser, or serve the folder with a lightweight local web server
3. Verify all pages load and the images are present
4. Check links to related pages and assets

Example local server:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Deployment

This project is intended for GitHub Pages deployment. Recommended deployment pattern:

- Keep all static pages in the repository root
- Use relative links between pages so the site remains portable
- Store screenshots and evidence files in the same repo for auditability
- Publish from the default branch configured in GitHub Pages
- Include a visible update date on the homepage and key pages

## Repository structure

```text
.
├── index.html
├── timeline.html
├── brunner-case.html
├── evidence/
│   └── index.html
├── *.jpg
├── *.png
├── robots.txt
├── sitemap.xml
├── googlefc161b35871c0f07.html
└── README.md
```

## Recommended maintenance practices

- Review the site monthly or after major updates to public records
- Keep evidence dates visible and consistent
- Validate that links remain correct after content updates
- Prefer plain-language explanations over legalistic wording
- Continue to make claims traceable to public sources

## Final recommendation

This project should remain intentionally simple, transparent, and low-maintenance. A static-site model is a strong fit because it is low cost, easy to audit, easy to publish, and reduces operational complexity. The core objective is to make public warning information understandable and verifiable without introducing unnecessary technical overhead.

This repository is best treated as a public-information archive and consumer-warning page, not as a full application platform.

## Disclaimer

This project is designed to organize publicly available information in a readable format. It is not a substitute for legal advice, formal background checks, regulatory review, or professional due diligence. Always verify information independently before making a financial, legal, or consumer decision.
