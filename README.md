# SnackSmart website

Production: https://gautam-u.github.io/snacksmart-website/

The homepage (`index.html`), support (`support/index.html`) and privacy (`privacy-policy/index.html`) pages are static HTML, served by GitHub Pages. Existing Terms of Service remain in `terms.md`, rendered through the shared Jekyll layouts. The deployment paths are unchanged.

`assets/site-v2.css` provides the shared responsive design. `assets/gallery.js` switches local screenshots and captions only; it does not send analytics. Without JavaScript the first screenshot and full-size image link still work.

`assets/screenshots-current/source-manifest.json` records screenshot sources and app version. Release-candidate screens are labeled on the homepage; do not imply they are already in the public store version.

Preview static pages with an HTTP server mounted at `/snacksmart-website/`. GitHub Pages also builds the existing Jekyll terms page. Check desktop and phone layouts, screenshot controls and support/privacy/terms navigation before publishing. Preserve app-ads.txt where present.
