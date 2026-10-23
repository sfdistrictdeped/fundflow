# FundFlow Beta 0.6.0 — GitHub Offline Package

## Deploy to GitHub Pages
1. Extract this folder.
2. Upload **all files in this folder** to the root of your GitHub Pages repository (or copy the contents into the intended subfolder).
3. Enable GitHub Pages for the branch/folder containing `index.html`.
4. Open the published HTTPS URL once while online so the service worker can install and cache the app shell.
5. Reopen the URL after the first load to use the cached app offline.

## Included
- `index.html` — FundFlow application, with embedded application logic and templates.
- `manifest.webmanifest` — installable PWA metadata.
- `sw.js` — service worker for app-shell/offline caching.
- `FundFlow_App_Icon.png` — app icon.
- Latest purchase and travel Excel template files for package completeness.

## Notes
- Service workers require HTTPS (GitHub Pages provides HTTPS) or localhost.
- Offline availability begins after the app has been opened successfully online at least once. Browser storage clearing, private browsing restrictions, or device policies can remove/limit the cache.
- This is a static GitHub Pages package; no server-side backend is required for the bundled client-side workflows.
