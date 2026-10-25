# Kinsay legal pages

Static legal documents for Kinsay, operated by Joe. Public contact:
heyjoewynn@gmail.com. Effective date: October 25, 2026.

Only the contents of this directory belong in the public legal repository.
App source, configuration, credentials, migrations, and internal product documents
are not part of the legal website.

## Published URLs

- Home: https://xubangbang.github.io/kinsay-legal/
- Privacy Policy: https://xubangbang.github.io/kinsay-legal/privacy.html
- Terms of Service: https://xubangbang.github.io/kinsay-legal/terms.html

## Hosting

Repository: https://github.com/xubangbang/kinsay-legal

Use GitHub Pages → Deploy from a branch → `main` → `/(root)`.
`.nojekyll` makes this an ordinary static HTML site. There is no build step,
JavaScript, tracking, external font, form submission, or app backend connection.
Relative links work under the repository's GitHub Pages path.

For local preview, run `python3 -m http.server 8765 --bind 127.0.0.1` from this
directory, then open http://127.0.0.1:8765/.

## Maintenance

Update both document dates when their substance changes. Keep these documents
aligned with the shipped app and actual provider configuration. In particular:

- Google sign-in SDK declarations include Analytics, linked identifiers/usage and
  other categories. Do not claim the absence of all third-party analytics. See
  `docs/app-privacy.md` in the app repository for the release disclosure worksheet.
- Account deletion deletes created Spaces and permanently erases the person’s
  original text in every other Space, even Spaces they have left. Empty deleted
  placeholders preserve other people’s reply links.
- Leaving a Space does not delete content. Reply deletion removes the text while
  preserving a placeholder when needed for other replies.
- The service is described as free, without advertising, sale of personal data,
  with provider sign-in analytics disclosed in the Privacy Policy. The minimum age is 13 or the higher local minimum,
  with guardian agreement for minors. Update these statements if practices change.
- The operator supplied the name Joe and the contact above. No operator country
  was supplied, so the Terms preserve applicable law and mandatory consumer rights
  without inventing an exclusive jurisdiction. Country-specific disclosures and
  legal review may be needed for the markets where the app is distributed.
- Confirm provider regions, email delivery arrangements, backup/log retention,
  and applicable international transfer safeguards as deployment settings change.
- Publishing these pages does not add in-app links, an acceptance flow, age
  verification, export, or moderation features. App Store privacy metadata and
  review requirements must match actual app behavior independently.

Drafted against the checked-in app and these official references:

- Apple App Review Guidelines, section 5.1.1:
  https://developer.apple.com/app-store/review/guidelines/#privacy
- ICO privacy notice guidance:
  https://ico.org.uk/for-organisations/advice-for-small-organisations/privacy-notices-and-cookies/cookies-and-privacy-notices-in-detail/
- GitHub Pages setup:
  https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- Provider privacy policies linked from the Privacy Policy.
