MISSION 17 — Android-friendly habit tracker

FILES
- index.html: the full app
- manifest.json: install metadata
- sw.js: offline app shell
- icons/: app icons
- README.txt: setup instructions

IMPORTANT
The app stores habit records in this browser's localStorage. It does not sync to the cloud or another device. Export a JSON backup from the Backup tab occasionally. Do not clear the browser's site data unless you have a backup.

EASIEST ANDROID INSTALL (recommended)
1. Extract the ZIP.
2. Upload the contents of the mission17_tracker folder to a static HTTPS host such as GitHub Pages or Netlify. Keep the folder structure intact. Do not upload the ZIP itself as the website.
3. Open the published HTTPS URL in Chrome on Android.
4. Tap Chrome's three-dot menu (⋮), then choose "Install app" or "Add to Home screen" and confirm.
5. Open Mission 17 from your home screen. Tick a habit; close and reopen the app to verify that it is saved.

GitHub Pages quick path
1. Sign in to GitHub and create a new repository (e.g. mission17).
2. Upload index.html, manifest.json, sw.js, the README and the icons folder to the repository root.
3. In repository Settings > Pages, enable deployment from the main branch and root folder.
4. Wait for GitHub Pages to publish the HTTPS site, then open the provided URL on your phone and install it from Chrome.

Daily reset and history
The app uses your phone's local calendar date. When the date changes, the checklist shows a fresh day automatically. Previous records stay in History and count toward the weekly report. A streak day means 80% or more of the 12 habits are complete.

DATA
- Ticks and reflections save locally as you interact.
- Use Backup > Export backup regularly.
- To move devices or restore after browser storage is lost, use Backup > Restore a backup.
- Import merges date records by date; if the same date exists in both backups, the imported version for that date replaces the existing version.

This is a Progressive Web App. Installability requires serving it from HTTPS (or localhost during development); opening index.html directly from a file manager is fine for a quick preview but will not provide full PWA installation/offline behavior.
