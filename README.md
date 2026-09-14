# Redwood Count

Installable job-sheet counter for **Redwood Electric**. Open it on an iPhone or iPad and Add to Home Screen, or Install on Android. Counts stay on the device (`localStorage` key `re-count-v2`).

**Live app:** https://redwoodelectricutah-dev.github.io/Redwood-Electric-count-app/

## Enable GitHub Pages (one click)

This repo is a static site at the **repository root**. Pages is not always on for a new repo.

1. Open **Settings → Pages**
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)**
4. Save

After a minute or two the app is at:

`https://redwoodelectricutah-dev.github.io/Redwood-Electric-count-app/`

If the repository is **private**, either make it **public** or use a GitHub plan that allows Pages on private repos. The Pages API is not writable from this setup, so the Settings toggle has to be clicked by a repo admin.

## Install on iPhone / iPad

1. Open the Pages URL in **Safari** (not Chrome or in-app browsers)
2. Tap **Share**
3. Tap **Add to Home Screen**
4. Confirm **Add**

Hint text in the app: *Open in Safari → Share → Add to Home Screen. Templates and jobs stay on this iPad.*

## Install on Android

1. Open the Pages URL in **Chrome**
2. Tap the menu (three dots) → **Install app** or **Add to Home Screen**, or use the Install banner
3. Confirm **Install**

## Using the app

- **Folders:** Jobs and Templates (plus any folders you create)
- **Templates:** column items and default rows — seed includes *Residential rough-in* and *Trim / devices*
- **Jobs:** rows × item counts with +/−, sticky header row
- **CSV** and **Print** from a job sheet
- Data never leaves the device; offline works after the first visit (service worker caches the app shell)

## Files

| File | Role |
| --- | --- |
| `index.html` | App UI and logic |
| `manifest.webmanifest` | PWA name, standalone display, theme `#1a2e24`, `start_url` `./` |
| `sw.js` | Caches the shell for offline; does not touch `localStorage` |
| `icon-192.png` / `icon-512.png` | Home-screen icons (RE, copper on dark green) |
