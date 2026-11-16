# My Budget (standalone)

A private budget app. All data stays on the device you use it on. There is no account, no cloud and no tracking, and the app is blocked from contacting anything except its own files.

## What's in this folder

| File | What it is |
| --- | --- |
| `index.html` | The whole app |
| `sw.js` | Lets it work with no connection |
| `manifest.webmanifest` | Lets it be added to the Dock or Home Screen |
| `icon-*.png`, `apple-touch-icon.png` | App icons |

None of these files contain any of your financial data, so they are safe to host publicly.

## Try it straight away

Double-click `index.html`. It opens in your browser and works. This is fine for a look, but for everyday use host it (below) so it can be installed and works offline on your iPhone too.

## Put it online with GitHub Pages (about five minutes, once)

1. Sign in at github.com and create a new repository. Name it `my-budget`, set it to Public, and create it.
2. On the new repository page choose "uploading an existing file", drag in every file from this folder, and commit.
3. Go to Settings, then Pages. Under "Build and deployment" choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. After a minute or two your app is at `https://YOUR-USERNAME.github.io/my-budget/`.

## Install it

- **Mac, Safari:** open the link, then File menu, Add to Dock.
- **Mac, Chrome:** open the link, then the install icon at the right of the address bar.
- **iPhone:** open the link in Safari, tap Share, then Add to Home Screen.

## Bring your data in

Open the app, tap "Bring in a backup file" and choose `my-budget-backup-2026-11-16.json`. Do this once on the Mac and once on the iPhone.

## Keeping Mac and iPhone in step

They do not sync by themselves, because that would need a server. To move data across:

1. On the device with the newest data: Backup & data, then Save a backup file.
2. AirDrop the file to the other device, or save it to iCloud Drive.
3. On the other device: Backup & data, Choose a backup file, then Merge.

Merge adds any spends and balance updates the other device is missing, and keeps whichever plan was edited most recently. The simplest habit is to log spends on your iPhone and merge into the Mac when you do your monthly check.

## Good to know

- Each browser keeps its own copy. Safari and Chrome on the same Mac do not share data, so pick one.
- Clearing website data for the site in your browser erases the app's data. Keep a recent backup file.
- To update the app later, replace `index.html` in the repository. Your data is not touched. If you change the files, raise the version in `sw.js` (`my-budget-v1` to `my-budget-v2`).
- Search: Cmd+K on a Mac, or the magnifying glass on iPhone.
