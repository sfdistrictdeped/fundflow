# FundFlow Beta 0.6.1 — GitHub Offline Package

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


## App icon and favicon (Beta 0.6.1 patch)
The package includes `favicon.ico`, `favicon.png`, `apple-touch-icon.png`, `icon-192.png`, and `icon-512.png`. The manifest references the 192px and 512px icons, and the service worker caches these assets. After replacing the files on GitHub Pages, open the app online once to refresh the cache. Windows may retain an installed app icon; if so, uninstall and reinstall the PWA.


## Beta 0.6.1 fixes
- Itinerary `G15`: employee position; `G16`: school name.
- Travel workbook removes the Travel Order when the memo already serves as the TO.
- Travel workbook removes the Locator Slip when not requested.
- BES and PFS sheets are omitted for now.
- Travel workbook generation always asks for a filename before downloading.
- Purchase workbook retains only the selected DV sheet.
- Uses the newly supplied `MOOE FOR TRAVEL TEMPLATE BLANK.xlsx`.

### Beta 0.6.1 patch — COTC date and date-picker visibility
- COTC `B20` is populated with the latest chronological date in the employee's itinerary.
- Itinerary and CENRR calendar picker indicators use visible green styling in light mode and a light-green indicator in dark mode.
- Version remains Beta 0.6.1.
