# gDAS Survey Logger PWA

Offline-capable sensor survey logging app for gDAS32 field deployments.

## Deploy to GitHub Pages (5 minutes)

1. Create a new GitHub repository (e.g. `gdas-survey`)
2. Upload ALL files from this folder maintaining the structure:
   ```
   index.html
   manifest.json
   service-worker.js
   icons/
     icon-192.png
     icon-512.png
   ```
3. Go to **Settings → Pages**
4. Under "Source", select **Deploy from a branch**
5. Choose **main** branch, **/ (root)** folder
6. Click **Save**
7. Wait ~1 minute, your app will be at: `https://YOUR-USERNAME.github.io/gdas-survey/`

## Usage

1. Open the URL on your phone in Chrome/Safari
2. GPS will work automatically (HTTPS gives permission)
3. Go to **Settings** tab → import your sensor plan .xlsx
4. Set **Datum** and **UTM Zone** on the Map tab
5. Start logging! All data stored locally on device
6. Export logs as .xlsx or .csv when ready

## Offline

After first load, the service worker caches everything.
The app works fully offline - form, logs, export all work without internet.
Map tiles are cached as you view them - previously viewed areas work offline.

## Adding to Home Screen

- **Android Chrome**: tap ⋮ menu → "Add to Home Screen"  
- **iPhone Safari**: tap Share → "Add to Home Screen"

This gives you a full-screen app experience with GPS.
