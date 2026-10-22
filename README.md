# VibezZzCoder Arcade & URL redirects

Public arcade: https://vibezzzcoder.github.io/

This repository hosts the account's root GitHub Pages site. Games remain in their own repositories and retain their own licenses and credits. The homepage lists only browser games whose Pages endpoints were verified live on 2026-10-22.

## Hosting

GitHub Pages publishes `main` / `(root)`. `.nojekyll` keeps these static files unchanged. No package installation or build is required.

## Existing redirect

| Old Pages path | Destination |
| --- | --- |
| `/usaf-hangar-fighter/` | `https://vibezzzcoder.github.io/hangar-fighter/` |

The old path is a directory in THIS repository, not a separate repository. **Never recreate a repository named `usaf-hangar-fighter`**: doing so would replace GitHub's automatic repository/Git redirects.

GitHub does not automatically redirect a renamed project's Pages URL. After the project rename, the root site serves `usaf-hangar-fighter/index.html`. It provides an immediate JavaScript replacement navigation (preserving query and fragment), a no-JavaScript meta-refresh, a canonical URL and a readable link. This is a static HTML redirect served with HTTP 200, not a server-side 301.

## Preserved legacy file links

The former site's three scenario PNGs and GPL `LICENSE` are retained byte-for-byte under `usaf-hangar-fighter/`; its README is retained there with the current game name and play link. This also keeps direct file links and README-relative screenshot links working. Those game files retain the game's existing GPL terms and attribution.

## Add a future game redirect

1. Verify the new game URL is deployed and works.
2. Copy `usaf-hangar-fighter/index.html` to `old-game-slug/index.html`.
3. Change every destination in the script, meta-refresh, canonical and visible link to the same trusted HTTPS URL. Use a fixed destination; never accept a URL from query parameters.
4. Update the game title, this table, and the arcade card.
5. Commit to `main` and wait for the Pages deployment.
6. Test the old path in a fresh browser, its `index.html` form, and with JavaScript disabled. Check that the HTTP response contains the redirect page rather than a 404.
7. Retain the directory permanently and keep the old repository name unused.

Do not add a root `CNAME` or change the account's Pages domain without reviewing the effect on ALL project sites. A catch-all 404 redirect is deliberately unnecessary: explicit old paths return a real page, and unrelated missing paths remain missing.
