# The System — install on your Pixel with a permanent URL

## 1. Get a permanent URL with GitHub Pages (free, stays live indefinitely)

1. Go to github.com and sign in (create a free account if you don't have one).
2. Click **+** (top right) → **New repository**. Name it something like `the-system-app`. Keep it Public. Create it.
3. On the new repo page, click **"uploading an existing file"** (or drag-and-drop).
4. Drag in all 6 files from this folder: `index.html`, `manifest.json`, `service-worker.js`,
   `icon-192.png`, `icon-512.png`, `icon-512-maskable.png`. Commit the changes.
5. Go to the repo's **Settings** tab → **Pages** (left sidebar).
6. Under "Build and deployment", set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
7. Wait ~1 minute, then refresh — GitHub shows your live URL, something like:
   `https://<your-username>.github.io/the-system-app/`

This URL is permanent — it stays up as long as the repo exists, and updating the files
in the repo updates the live app.

## 2. Install it on your Pixel

1. Open that URL in **Chrome** on your Pixel.
2. Tap the **⋮ menu** → **Install app** (or "Add to Home screen").
3. It now sits on your home screen and opens full-screen, like any other app.

## 3. Keeping your data safe (important)

Your entries are saved in that copy of Chrome's local storage — not in the cloud. That means:
- Clearing Chrome's site data/history for this app wipes your entries.
- The data won't automatically appear if you open the app on a different phone or browser.

To protect against that, open the app's **Settings** (bell icon) → **Backup & restore**:
- **Download backup (.json)** — saves a file with every goal, check-in, and weekly review.
  Save this to Google Drive, email it to yourself, or store it wherever you keep other
  important files. Do this every so often (e.g. weekly, right after your weekly review).
- **Restore from backup file** — pulls a previously downloaded file back into the app.
  Use this if you clear your browser data, switch phones, or reinstall the app — your
  full history comes back exactly as it was.

There's no automatic cloud sync in this version — the backup file is your safety net.
If you'd like true automatic cloud sync (so entries sync live across devices without
manual backups), that requires wiring the app up to a real backend service — let me
know and I can help set that up.
