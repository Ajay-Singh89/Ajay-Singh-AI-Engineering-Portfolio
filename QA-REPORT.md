# Portfolio QA — 7 review iterations

## Final reviewer score: 9.4/10 (design/content/code review)
This is a static QA and design-review score, not a claim that a real browser automation agent completed end-to-end tests. The environment blocked Chromium navigation (`ERR_BLOCKED_BY_ADMINISTRATOR`), so interactions that require a real browser should be rechecked after deployment.

## Iteration log
1. **Content accuracy (8.4/10):** Matched the portfolio to the supplied résumé; avoided inventing project metrics or unverified demo URLs.
2. **Recruiter story (8.7/10):** Reworked the opening around AI engineering, RAG, secure tool use, and backend development; made internship interest visible.
3. **Project scanability (8.9/10):** Added four consistent project cards with concise descriptions and stack tags.
4. **Visual hierarchy (9.1/10):** Added dark editorial styling, clear typography, abstract technical visuals, section rhythm, and hover states.
5. **Responsive layout (9.2/10):** Added mobile navigation and breakpoints; added a reduced-motion preference.
6. **Functional controls (9.3/10):** Implemented theme toggle, mobile menu state, email copy with fallback message, scroll progress, active-section navigation, resume link, mailto/tel links.
7. **Final QA and polish (9.4/10):** Corrected/checked section anchors and local asset paths, confirmed unique HTML IDs, validated JavaScript syntax, and ensured the résumé PDF is packaged.

## Automated checks passed
- HTML parser accepted the document.
- 15/15 static checks passed: unique IDs, valid in-page anchors, local links resolve, four project cards, all major sections, responsive breakpoint, reduced-motion support, accessible navigation state, theme and copy handlers, scroll progress, résumé PDF, SEO description, email and phone links.
- `node --check script.js` passed.

## Browser testing limitation
A Playwright browser launch was attempted, but Chromium navigation was blocked by the execution environment. Therefore clipboard permissions, visual rendering across actual browsers, and mobile interactions have not been independently confirmed in a live browser session. Re-test these after publishing.
