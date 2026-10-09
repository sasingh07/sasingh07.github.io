# Change 2 — Agent Sergeant project preview

**Status:** Revised proposal; awaiting approval. No project content has been added to the website.

## Objective

Introduce Agent Sergeant as a project currently being built, while keeping public information limited. Complement the portfolio's data, finance, valuation, and technology positioning without implying a launched product or proven capabilities.

## Source and disclosure boundaries

Based on the supplied **Agent Sergeant — Gate 1 Executive Summary**, which describes a project aimed at verifying AI agent behavior against enterprise rules.

- Share the project name, broad problem, intended approach, and in-development status only.
- Use first-person wording about what the user is building. Do not mention team involvement or collaborators; do not imply sole authorship or invent a specific technical role.
- Describe proposed capabilities as aims, not completed or validated functionality.
- Do not add the uploaded document to the public website or provide a download link.
- This supplied project extends Change1's résumé-only content scope for this feature; its other accuracy and design constraints remain in place.

## Proposed placement and design

Add one compact **Currently Building** section to `index.md`, after Selected Experience and before Beyond the Work.

- Heading: **Agent Sergeant**.
- Visible status: **In development**.
- One short paragraph, approximately 50 words; no expandable case study or detailed feature list.
- Open with the problem that makes the project interesting, then connect it to what the user is building. Keep the tone engaging and personal rather than sounding like a product specification.
- Reuse the existing single-column layout, thin dividers, navy/blue palette, and system-driven light/dark themes.
- Give the status a text label rather than relying on color alone.
- Do not make the section appear clickable when there is no supplied public project destination.
- Leave the existing professional highlights and primary actions unchanged.

No new Projects page or navigation item is needed for this initial preview.

## Proposed public copy

**Currently Building**

### Agent Sergeant

**In development**

> An AI agent can give the right answer—and still skip a critical check. I’m building Agent Sergeant to explore that gap with deterministic checks against approved rules. The goal: make deviations visible and give people clear evidence to review, instead of leaving them to dig through logs.

This is the complete proposed public description, not an introduction to a longer case study.

## Details to omit

- Market statistics, adoption figures, purchase-intent estimates, and account/opportunity calculations.
- Competitive comparisons, commercialization claims, and claims of market leadership.
- Detailed Read / Check / Prove workflows, inputs, permissions, schemas, architecture, deviation scoring, and auditor-report specifications.
- Guarantees about enterprise-data privacy, security, compliance, or deterministic correctness.
- Customer names, deployment claims, traction, performance metrics, timelines, or completed milestones.
- Unverified stack choices, integrations, screenshots, demos, repositories, or precise individual responsibilities.

## File scope

| File | Change |
| --- | --- |
| `Change2.md` | Record this proposal; after approval, document implementation and actual verification results. |
| `_config.yml` | Exclude `Change2.md` from generated output immediately, as with existing planning documents. Preserve all other configuration. |
| `index.md` | After approval, add the compact Currently Building section and the approved copy. |
| `assets/css/style.css` | After approval, add only minimal section/status styling if existing styles are insufficient. |

The planning-file exclusion is a publication safeguard, not implementation of the proposed project section.

## What stays unchanged

- Existing Home, About, Work Experience, and Contact routes and navigation.
- Résumé content, employment accomplishments, biography, and contact details.
- Root-level Jekyll, Markdown with YAML front matter, GitHub Pages configuration, and URL filters.
- No JavaScript, framework, backend, additional dependencies, external fonts, tracking, or project application embedded into this portfolio.
- No publishing or GitHub deployment as part of this change.

## Implementation and verification after approval

1. Add the approved copy to the Home page with a semantic section and heading.
2. Reuse the existing visual conventions and add only necessary responsive CSS.
3. Confirm the section is labeled Currently Building, omits team references, and uses engaging first-person copy while presenting capabilities as goals rather than completed functionality.
4. Build Jekyll and restart the preview once after the website edits.
5. Check the Home page at 375px and 1280px in both themes, including heading order, status readability, focus, contrast, and horizontal overflow.
6. Check existing navigation, internal links, work-highlight anchors, and contact links for regressions.
7. Run Lighthouse on the updated Home page, targeting at least 90 for Performance, Accessibility, Best Practices, and SEO; record actual results.
8. Confirm that `Change2.md` and all uploaded PDFs are absent from generated output.

## Approval

Awaiting approval of the placement, scope, and proposed public copy before any website-content or design implementation.
