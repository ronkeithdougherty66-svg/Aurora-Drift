# Aurora Drift — GitHub Pages setup

This folder is a complete installable web app (PWA). Once it's hosted on
GitHub Pages (which serves over `https://`), "Add to Home Screen" on
Android will install it as a real standalone app — full screen, its own
icon, no browser address bar.

## Steps

1. Go to https://github.com and sign in (or create a free account).
2. Click the **+** in the top right → **New repository**.
   - Name it anything, e.g. `aurora-drift`.
   - Set it to **Public** (required for free GitHub Pages).
   - Click **Create repository**.
3. On the new repo's page, click **Add file → Upload files**.
4. Drag in all 5 files from this folder:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
5. Click **Commit changes**.
6. Go to the repo's **Settings** tab → **Pages** (left sidebar).
7. Under "Build and deployment" → **Source**, choose **Deploy from a
   branch**. Under "Branch," choose `main` and folder `/ (root)`. Click
   **Save**.
8. Wait about 1–2 minutes. Refresh the Pages settings screen — it will
   show a link like:
   `https://yourusername.github.io/aurora-drift/`
9. Open that link on your Android phone in **Chrome**.
10. Tap the **⋮** menu → you should now see **"Install app"** or **"Add
    to Home Screen"** — this time it will install as a real standalone
    app with the orb icon, not just a bookmark.

That's it — the app now lives on your home screen and also works
offline after the first load, since the service worker caches it.
