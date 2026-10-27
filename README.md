# Wardrobe Lookbook

A personal wardrobe app that runs in Safari and installs to the iPhone Home Screen.

This folder holds only the app's code. It contains no clothes, photos or outfit looks, so it is safe to publish.
Your wardrobe (pieces, photos, looks and colour guide) comes from a private file, `wardrobe-data.json`, that you
load on your phone. The app copies it into the phone's own storage. It is never uploaded anywhere.
Everything you add in the app (pieces, saved looks, ratings, wear log) also stays on the phone.

**Never put `wardrobe-data.json` or a backup file in this folder or in the GitHub repository.**

## Put the app online for free (GitHub Pages)

1. Create a free account at https://github.com/signup.
2. Click **+** (top right) → **New repository**. Name it `wardrobe`, leave it **Public**, and click **Create repository**.
3. On the empty repository page, click **uploading an existing file**.
4. In Finder, open this `wardrobe-app` folder, press **Cmd+A** to select everything inside it (including the `fonts`
   and `img` folders), and drag it all into the browser window. Wait until every file is listed (12 files), then click
   **Commit changes**.
5. Go to **Settings** → **Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**,
   **Branch** to `main` and the folder to `/ (root)`, then click **Save**.
6. Wait 1–2 minutes and refresh. The page shows **Your site is live at** `https://YOUR-USERNAME.github.io/wardrobe/`.

## Install on your iPhone

1. Open that link in **Safari** and let the page finish loading.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open the app from the new icon. It asks for your wardrobe file.
4. Send `wardrobe-data.json` to your phone (on the Mac: right-click → **Share** → **AirDrop**), then tap
   **Load wardrobe file** and pick it. After that the app works offline, and you can delete the file from your phone.

## Keep your data safe

Your wardrobe lives only on that phone. Use **Hub → Save backup** now and then and save the file to Files or iCloud Drive.
The backup includes everything: your wardrobe, photos, colour guide, and what you added. On a new phone, install the app
and tap **Restore from backup** on the first screen.

## Updating the app later

Upload the changed files to the repository the same way (they replace the old ones), and change
`wardrobe-v3` at the top of `sw.js` to `wardrobe-v4` (then v5, and so on). Close and reopen the app on your phone
to get the new version. Your saved data is kept.

To update your wardrobe itself (new photos, renamed items, new looks), load a newer `wardrobe-data.json` in
**Hub → Wardrobe file**. That keeps everything you added in the app.
