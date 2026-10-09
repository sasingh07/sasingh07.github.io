# Change 1 — Data, finance, valuation, and technology

**Status:** Approved, implemented, and verified.

## Objective

Refine Saurabh Singh's portfolio so it reads as the professional site of someone with experience in financial analysis, valuation, economic consulting, secondary-market investing, and technology-related work. Keep it personal, credible, and easy to scan rather than making it resemble a trading platform or a generic technology startup.

## What needs to improve

- The current oversized greeting and generous empty space make the homepage primarily an introduction. Relevant experience and analytical capabilities should be visible earlier.
- The warm green palette is approachable but does not strongly distinguish the site's analytical focus.
- Experience is presented as long résumé lists. Employers, role progression, analytical methods, and outcomes need clearer visual hierarchy.
- Data and technology experience is present in the content but is not immediately apparent from the homepage.
- The homepage should say **MBA candidate at Berkeley Haas**, not imply that the MBA has already been completed.

## Proposed visual direction

### Palette

- Replace the cream-and-green emphasis with a restrained ink/navy, cool neutral, and blue palette.
- Proposed light theme: off-white background (`#F8FAFC`), deep navy text (`#0F172A`), blue links and primary actions (`#1D4ED8`).
- Proposed dark theme: navy background (`#0B1220`), light text (`#E2E8F0`), lighter blue accents (`#93C5FD`).
- Use teal sparingly for analytical labels, not as the main brand color.
- Final color pairs must pass contrast checks in both themes. Do not rely on color alone to identify links, active navigation, or categories.

### Typography and spacing

- Keep locally available system sans-serif fonts; do not introduce third-party font requests.
- Reduce the large name heading to approximately 56–72px on desktop and 36–44px on mobile, with responsive sizing.
- Keep body text at least 16px, comfortable line spacing, and readable line lengths.
- Use restrained monospace styling for dates and numerical labels, with tabular numerals for financial figures where supported.
- Reduce excessive top padding so positioning and a clear experience link appear within the initial viewport.
- Preserve the responsive, single-column layout. Use thin dividers and consistent section spacing rather than oversized cards, dense dashboards, or decorative grids.

### Navigation and brand

- Keep the name as the primary identity and retain the four existing pages.
- Use the full **Work Experience** label where space permits, wrapping cleanly on narrow screens.
- Refine the existing monogram and favicon into a consistent, simple mark.
- Retain visible keyboard focus, the skip link, active-page indication, and semantic navigation.

## Page-by-page changes

### Home

1. Keep the name prominent, but make professional positioning equally clear.
2. Proposed positioning: **Financial analysis, valuation, and technology-informed investing.**
3. Support it with factual copy naming Berkeley Haas MBA candidacy, CRA economic consulting, and Ponte Partners secondary-market experience.
4. Make **View work experience** the primary action and **Get in touch** the secondary action.
5. Add a compact, stacked expertise section:
   - **Data & analysis:** financial and industry research, scenario analysis, and risk-adjusted pricing models.
   - **Finance & valuation:** investment due diligence, valuation, and litigation damages analysis.
   - **Technology context:** tech and AI sector research, healthcare SaaS analysis, and tools including Python, Claude Code, Bloomberg, and S&P Capital IQ.
6. Add two concise, contextualized work highlights linking to the Experience page: secondary-portfolio pricing at Ponte and valuation/damages analysis at CRA.
7. Retain personal interests lower on the page so the site still feels personal.

### About

- Lead with the connection between economics, analytical work, investing, and the current MBA.
- Separate education, tools, mentoring, and personal interests with consistent headings and spacing.
- State the MBA graduation date as **expected May 2027**.
- Present tools in a compact text list, retaining **intermediate** as the stated Python proficiency.
- Avoid skill-rating bars or invented proficiency levels.

### Work Experience

- Retain reverse chronological order: Ponte Partners, then CRA and its three roles.
- Introduce a restrained vertical progression with clear employer, role, location, and date hierarchy; keep all information in one reading column.
- Make existing bullets easier to scan by emphasizing the analytical work and its stated result.
- Use selected figures only with their explanation, not as detached promotional statistics.
- Where helpful, group the existing text under meaningful headings such as investment research, pricing, valuation, and damages analysis without adding unsupported responsibilities.
- Retain all substantive résumé accomplishments and dates; do not turn consulting engagements into invented standalone projects.

### Contact

- Keep email, LinkedIn, and GitHub as direct, accessible links.
- Align spacing, labels, and hover/focus styling with the revised design.
- Keep the phone number and uploaded résumé PDF unpublished.
- No contact form, backend, tracking, or new personal details.

## Content accuracy rules

- Use only the supplied résumé and already approved site content.
- Portfolio size is not a personal investment result. A 65% discount to NAV refers to investment committee approval of the bidding strategy, not a realized return or completed transaction.
- Preserve context around settlement amounts, claimed damages, and investment agreements; do not imply sole responsibility for team outcomes.
- Technology positioning must remain grounded in sector research, client work, and listed tools. Do not claim software engineering, data-science, or AI product-building credentials.
- Do not add charts with invented data, stock-market feeds, employer logos, client testimonials, or new projects.

## Implementation scope

| File | Planned change |
| --- | --- |
| `assets/css/style.css` | Update palette, typography, spacing, numerical styling, content hierarchy, and responsive rules. |
| `index.md` | Refine positioning, actions, expertise summary, and selected work highlights. |
| `about.md` | Improve the organization of the existing biography, education, tools, and interests. |
| `experience.md` | Improve role hierarchy and scanability while preserving sourced facts and dates. |
| `contact.md` | Align contact presentation with the refined design. |
| `_includes/header.html`, `_includes/footer.html` | Refine shared branding, navigation, and footer styling. |
| `_data/navigation.yml` | Adjust the experience navigation label if needed. |
| `_layouts/default.html` | Update theme-color metadata and add only reusable presentation hooks if needed. |
| `assets/favicon.svg` | Align the monogram with the revised palette. |
| `_config.yml` | Align the site description with approved positioning; keep this planning document excluded from publication. |
| `README.md` | Update editing guidance only if presentation conventions change. |

## What will not change

- Root-level Jekyll site with Markdown content and YAML front matter.
- Existing page routes, GitHub user-site URL, empty `baseurl`, and URL filters.
- Publishing from `main` and `/ (root)` through GitHub Pages.
- System-driven light/dark themes, SEO tags, sitemap, and favicon.
- No React, Vite, Node application, database, CMS, blog, external fonts, trackers, or animation system. No JavaScript is needed for the planned changes.

## Implementation and verification sequence

1. Apply the shared visual system and responsive spacing.
2. Refine the Home page, then About, Experience, and Contact.
3. Check all copy against the supplied résumé and preserve accurate qualifications.
4. Restart the Jekyll preview and confirm that the site builds successfully.
5. Check all four pages at 375px and 1280px in light and dark themes; verify no horizontal overflow or clipped navigation.
6. Check keyboard focus, heading order, contrast, active navigation, and all internal/contact links.
7. Re-run Lighthouse with a target of at least 90 in Performance, Accessibility, Best Practices, and SEO. Report actual scores and any unavailable checks.
8. Confirm that the complete source remains at repository root, no separate application exists, and neither this document nor uploaded source files appear in generated website output.

## Assumptions

- This is a refinement of the current four-page site, not a redesign into a multi-column dashboard.
- A navy/blue visual direction is proposed for approval; it is not a previously stated color preference.
- Professional positioning may be rewritten for clarity without adding qualifications or accomplishments.
- Publication to GitHub is outside this design change; no repository or live deployment will be modified without a separate request.

## Implementation record

- Replaced the warm green styling with the approved navy/blue light and dark palettes, a matching SS monogram/favicon, smaller headings, tighter spacing, and monospace/tabular date labels.
- Refined Home to lead with financial analysis, valuation, and technology-informed investing. Added the three expertise areas, two contextual work highlights, and links to the relevant Experience sections.
- Reorganized About into education, tools, mentoring, and personal sections. MBA candidacy and the expected May 2027 graduation date are explicit; Python remains intermediate.
- Introduced a restrained vertical work-history progression with clear employers, roles, locations, and dates. Preserved the résumé's financial figures and accomplishments and clarified the NAV discount as bidding-strategy approval.
- Aligned Contact and shared navigation/footer styles. The email, LinkedIn, and GitHub links remain direct links; uploaded source documents stay excluded from publication.
- No new pages, executable JavaScript, external fonts, charts, application framework, or backend were added.

### Verification results — October 8, 2026

These checks used the local Jekyll preview, not a published GitHub Pages deployment.

| Page | Performance | Accessibility | Best Practices | SEO |
| --- | ---: | ---: | ---: | ---: |
| Home | 100 | 100 | 100 | 100 |
| About | 100 | 100 | 100 | 100 |
| Work Experience | 99 | 100 | 100 | 100 |
| Contact | 100 | 100 | 100 | 100 |

- Jekyll build and whitespace/diff checks passed.
- Checked all four pages at 375px and 1280px in light and dark themes: all 16 combinations passed horizontal-overflow, navigation, heading-order, active-page, and keyboard skip-link checks.
- Inspected rendered desktop/mobile layouts and the dark contact page. Checked the defined text, link, label, and button color pairs in both themes; each exceeded the 4.5:1 normal-text contrast requirement.
- Internal links and work-highlight anchors resolve; no placeholders appear in rendered pages.
- Financial figures and role dates remain present in the generated Experience page.
- Confirmed the source site remains at repository root and the output contains only website pages and assets. Planning documents and uploaded PDFs are excluded.
- Temporary browser/audit tools are not part of the website or its GitHub Pages build.

### Deployment status

The local design update is complete. GitHub publishing was not performed as part of this change.
