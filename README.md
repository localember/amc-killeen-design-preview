# AMC Killeen location site: Design preview, not live

Ticket AMC-2026-11-25-killeen-site-build. Built the same way as amc-copperascove-design-preview, including the
Nov 25 review changes: button hover, menu matching this location's live menu minus Home, scroll-away
header + sticky bottom CTA, Short Answer stock images on service and condition pages.

Full Killeen location site on the AMC main design (Local Ember Alpine, AMC palette). Every URL on
the live killeen.anthonychiro.com site (sitemap and the live menu) is kept at the same slug so rankings
can carry over, except /additional-offers/ and /ai-generated-content-disclaimer/, removed on John's
instruction (same as the Copperas Cove preview). Additional Promotions is left out of the menu with that page.

- noindex,nofollow on every page and robots.txt Disallow: /
- Forms off: disabled inputs and buttons, no form actions, no tracking or third-party scripts
- Service and condition pages use the Local Ember catalog (tools/bd-generator/catalog), carried through the Copperas Cove / Georgetown pattern. Acupuncture pages use services/acupuncture.json. Medical weight loss does not use services/weight-loss.json, because that file is a non-medical program and says not to extend it. Those pages carry the current Killeen wording.
- Blog: 2 posts rewritten as the pattern (car-accident-tips-chiropractor, sciatic-leg-pain); remaining placeholders at their exact live URLs
- Legal pages are the Local Ember standards, at the live site's slugs, plus the Texas Consumer Notice standard
- Review layer: assets/review-comments.js adds a Local Ember reviewer toolbar. It is not part of the site design and must not ship to the live site.
- Not the live site. Not sent to the client.
- Do not expand the homepage-only folder in amc-main-design-preview/killeen/.
