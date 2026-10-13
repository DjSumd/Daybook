# Daybook

A quick daily record of what you got done at work. Capture in a tap, search the whole archive, filter by month to plan the next year, and export a clean dated record whenever you need receipts.

Phone-first. No account, no cloud, works offline. Everything stays on the device.

## What's in here

```
index.html                 the whole app
manifest.webmanifest       makes it installable to the home screen
sw.js                      offline cache
icons/                     app icons
```

## Put it online (GitHub Pages)

1. Go to GitHub and create a new repository named **Daybook** (public).
2. Upload every file and folder in this bundle to the repo root (keep the `icons` folder as a folder).
3. In the repo: **Settings > Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**. Save.
4. Wait about a minute. The app goes live at:

   `https://djsumd.github.io/Daybook/`

## Install it on your phone

- **Android (Chrome):** open the link, tap the **⋮** menu, then **Add to Home screen** / **Install app**.
- **iPhone (Safari):** open the link, tap **Share**, then **Add to Home Screen**.

It then launches full screen like a normal app and runs offline.

## Using it

- **Today** is the capture screen. Type what you did, tap **Log it**. Start any word with `#` to tag it (optional, never required).
- **Archive** holds everything. Search, filter by month and year, tap a tag, or hit "This week, last year" when you're planning the same stretch of the year again.
- **Records** has your stats, a **printable record** (opens a clean dated log you can save as PDF or print), and **backup**.

## Backups matter

Because the data lives only on the phone, clearing the browser or uninstalling wipes it. Open **Records > Export backup** now and then and keep the `.json` file somewhere safe. **Restore from backup** brings it all back on a new device or after a reinstall.

## Updating later

Replace `index.html` (or whatever changed) in the repo. The version number in `sw.js` (`daybook-v1`) controls the offline cache. If you ever change cached files and an old version sticks, bump it to `daybook-v2` so phones pull the new files.
